# London Data
Spatial data for London, curated for analysis using [ONS geographies](https://www.ons.gov.uk/methodology/geography/ukgeographies). Python code used to manipulate data from original sources is [provided](https://github.com/jamesdamillington/london-data/tree/main/code) (along with a [file]() specifying package requirements).

## Geographies
Boundary data for various geographies the UK ONS uses to produce statistics (e.g. census, electoral). Provided in .shp and .csv format, usually with [BNG CRS]().

### Census
- [london2021-lsoa.shp]() - LSOA boundaries (original from ONS) with codes and names for LSOA, MSOA and LAD. [[Source Code]]()   
- [london2021-lsoa_simple.csv]() - as for [london2021-lsoa.shp]() but with simplified polygons for smaller file size. [[Source Code]]()  
- [london2021-lsoa_trunc.csv]() - as for [london2021-lsoa_simple.csv]() but with integer co-ordinates for even smaller file size. [[Source Code]]()
