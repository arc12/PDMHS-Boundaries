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

OS Parishes also contains some non-civil-parish entries. These appear in "parish_region" without names and have had sensible names added,  e.g. Buxton.

## From Cambridge Population and Social Structure

Hundreds are taken from "1831 England and Wales census hundreds and wapentakes GIS shapefile" by Max Satchell, obtained from the UK Data Service. Full citation:

> Satchell, M., Shaw-Taylor, L., Wrigley E.A.,1831 England and Wales census hundreds and wapentakes shapefile (2017). This dataset was created with funding from the ESRC (RES-000-23-1579), the Leverhulme Trust and the British Academy. The Satchell et al dataset derives from an enhanced version of Burton, N., Westwood J., and Carter P., GIS of the ancient parishes of England and Wales, 1500-1850. Colchester, Essex: UK Data Archive (May 2004), SN 4828, which is a GIS version of Kain, R.J.P., and Oliver, R.R., Historic parishes of England and Wales: An electronic map of boundaries before 1850 with a gazetteer and metadata. Colchester, Essex: UK Data Archive, May, 2001. SN 4348.  A description of the dataset can be found in Satchell, M., '1831 England and Wales census hundreds and wapentakes GIS documentation' (2017, 2006) available at:
> http://www.geog.cam.ac.uk/research/projects/occupations/datasets/documentation.html



Parishes and Places 1851:

> Satchell, A.E.M., Kitson, P.M.K., Newton, G.H., Shaw-Taylor, L., Wrigley E.A., 1851 England and Wales census parishes, townships and places (2016). This dataset was created with funding from the ESRC (RES-000-23-1579), the Leverhulme Trust and the British Academy. A description of the dataset can be found in Satchell, A.E.M., England and Wales census parishes, townships and places: documentation (2016, 2006) available at:
> http://www.geog.cam.ac.uk/research/projects/occupations/datasets/documentation.html



## Other Notes
The OS BoundaryLine shapefiles use original-precision data. This could be simplified in QGIS to give substantial file size reductions with only minor discrepancies. e.g. using 5m as the threshold for the simplification tool reduces the Parishes shapefile from 2.7M to 750k.

A layer called "PDMHS Area" has been created from a union of the selected OS Parishes, further subject to some truncation of the urban areas: Sheffield, Huddersfield, Stockport, E Manchester.
