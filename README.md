# WebmapsImmi

## Workflow

### Choropleth maps on asylum applications (abs/rel)
- Download world shapefile/geoJSON from the web (e.g. http://thematicmapping.org/downloads/world_borders.php)
- Download number of asylum applications and total population (both by country, 2008-2015) from Eurostat
- Do some preprocessing in R and save the pop/immi data as csv (mergeData.csv)
- Join in QGIS, export as geoJSON (alldata.geojson)

### ZEIT article replication
1. Downloaded data from https://docs.google.com/spreadsheets/d/1yxi3oV96kxag_3GiVnGvndgJ5zTI-lHsaAB-p7U-g3w/edit#gid=1734573181
   -> article link: http://www.zeit.de/politik/deutschland/2015-11/anti-immigrant-violence-germany
2. Use Python (GetCoord.ipynb) to get coordinates since spreadsheet does NOT contain latlng.
3. Steal incident type icons from original map (cf. article).
4. Use R to translate data set, summarize state of investigation, count within states, and make graphics.
5. Add new layers to map: incident type, state of investigation, summary per Bundesland.

### Make one more map (deaths and routes)?
