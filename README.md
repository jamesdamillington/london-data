# London Data
Spatial data for London, curated for analysis using [ONS geographies](https://www.ons.gov.uk/methodology/geography/ukgeographies). Python code used to manipulate data from original sources is [provided](https://github.com/jamesdamillington/london-data/tree/main/code) (along with a [file](https://github.com/jamesdamillington/london-data/blob/main/code/environment.yml) specifying package requirements).

## Geographies
Boundary data for various geographies the UK ONS uses to produce statistics (e.g. census, electoral). Provided in `.shp` and `.csv` format, usually with [BNG CRS](https://epsg.io/27700).

### Census
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/geographies/census) as follows:
- `london2021-lsoa.shp` - LSOA boundaries (original from ONS) for 2021 with codes and names for LSOA, MSOA and LAD. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)   
- `london2021-lsoa_simple.csv` - as for `london2021-lsoa.shp` but with simplified polygons for smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)  
- `london2021-lsoa_trunc.csv` - as for `london2021-lsoa_simple.csv` but with integer co-ordinates for even smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)
- `london2011-lsoa.shp` - LSOA boundaries (original from ONS) for 2011 with codes and names for LSOA, MSOA and LAD. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)   
- `london2011-lsoa_simple.csv` - as for `london2011-lsoa.shp` but with simplified polygons for smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)  
- `london2011-lsoa_trunc.csv` - as for `london2011-lsoa_simple.csv` but with integer co-ordinates for even smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)

## Population
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/population) as follows:
- `london-mid2020-pop.csv` - LSOA mid-year population estimates for 2020. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-population-midyear-estimates.ipynb)
- `london-mid2019-pop.csv` - LSOA mid-year population estimates for 2019. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-population-midyear-estimates.ipynb)
