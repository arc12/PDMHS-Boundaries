# PDMHS-Boundaries
Various externally-sourced and specifically-created boundaries for PDMHS geospatial database work.
Shapefiles all in the same directory as the QGIS project file. Maintain the data using the QGIS project "PDMHS Boundaries.qgz". There is also an experimental project "PDMHS Boundaries Cloud.qgz", which is __not__ for use, which is linked to the QGIS Cloud map accessible from:https://qgiscloud.com/arc12/PDMHS_Boundaries_Cloud. Only rudimentary QGIS styles are in place. The projects also include BGS bedrock overlay and an OpenTopoMap base map.

## PDNP Boundary
Extracted from https://geoportal.statistics.gov.uk/datasets/df607d4ffa124cdca8317e3e63d45d78_2
There are two shapefiles; the "Generalised 20m" one is much smaller and is generally very close to the actual boundary (23k vs 763k)

This is published under an Open Goverment Licence v3.0, for which the following attribution is required (see https://www.ons.gov.uk/methodology/geography/licences):  
"Contains National Statistics data © Crown copyright and database right [year]"  
"Contains OS data © Crown copyright and database right [year]"

## From OS BoundaryLine
Source: https://www.ordnancesurvey.co.uk/business-and-government/products/boundaryline.html, licenced under Open Government Licence, for which the attribution requirede is:  
"Contains OS data © Crown copyright and database right 2018"

Data extracted to cover PDNP, adjacent areas incl Ashover and Crich and Alderley Edge, and abutting or overlapping areas. The shapefiles/layer names (and the original boundary line shapefile name) areL
- OS Ceremonial Counties = "Boundary-line-ceremonial-counties"
- OS Districts = "district_borough_unitary_region"
- OS Parishes = "parish_region"

## Other Notes
The OS BoundaryLine shapefiles use original-precision data. This could be simplified in QGIS to give substantial file size reductions with only minor discrepancies. e.g. using 5m as the threshold for the simplification tool reduces the Parishes shapefile from 2.7M to 750k.
