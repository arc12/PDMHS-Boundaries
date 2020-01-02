# Notes on the Boundaries

## The PDMHS Area
The logic for the PDMHS area is to start with the National Park area and then to adjust the boundaries such that:
- Alderley Edge is included
- Churnet Valley iron is included
- a swathe from Ashbourne round via Wirksworth and Matlock, including Crich is included
- fringe areas of W Sheffield are included
- the area N of the A628 is excluded
- things are generally filled-in (e.g. the A6 corridor from Buxton)
- the boundary matches current OS Parish boundaries.

Following parishes is to allow for creating exports/views by Parish without unexpected areas with missing data caused by using the area boundary as a filter. The only clear case where this is unhelpful is Sheffield, for which we include the whole city.

The full extent in OSGB is:
381355, 340577, 445079, 402069  (Emin, Nmin, Emax, Nmax)

The covered 10km tiles are (organised as on map):
----, ----, ----, SE10, SE20, SE30, ----
----, SJ99, SK09, SK19, SK29, SK39, SK49
SJ88, SJ98, SK08, SK18, SK28, SK38, SK48
SJ87, SJ97, SK07, SK17, SK27, SK37, ----
----, SJ96, SK06, SK16, SK26, SK36, SK46
----, SJ95, SK05, SK15, SK25, SK35, SK45
----, SJ94, SK04, SK14, SK24, SK34, SK44

These are only thin slivers and can generally be neglected:
SE10, SE20, SE30
SJ88, SJ99, SK49
SK44, SK45, SK46

Additionally, SK48 is E Sheffield.

## Other Areas
### Parishes
The OS Parishes which match the PDMHS area are all included. 1851 Parishes are sometimes wierd and wonderful and do not match; a judgement call was made as to which were included, but in general, there are only very small missing holes and transgressions outside the PDMHS Area.

### Hundreds
Apart from a small area around Ripley, all the Hundreds covering the PDMHS Area are included. Most cover areas which are not in the PDMHS Area.