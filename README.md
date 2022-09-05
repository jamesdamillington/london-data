# London Data
Spatial data for London, curated for analysis using [ONS geographies](https://www.ons.gov.uk/methodology/geography/ukgeographies). Python code used to manipulate data from original sources is [provided](https://github.com/jamesdamillington/london-data/tree/main/code) (along with a [file](https://github.com/jamesdamillington/london-data/blob/main/code/environment.yml) specifying package requirements).

## Geographies
Boundary data for various geographies the UK ONS uses to produce statistics (e.g. census, electoral). Provided in `.shp` and `.csv` format, usually with [BNG CRS](https://epsg.io/27700).

### Census
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/geographies/census) as follows:
- `london-2021-lsoa.shp` - LSOA boundaries (original from ONS) for 2021 with codes and names for LSOA, MSOA and LAD. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)   
- `london-2021-lsoa-simple.csv` - as for `london-2021-lsoa.shp` but with simplified polygons for smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)  
- `london-2021-lsoa-trunc.csv` - as for `london-2021-lsoa-simple.csv` but with integer co-ordinates for even smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb)
- `london-2011-lsoa.shp` - LSOA boundaries (original from ONS) for 2011 with codes and names for LSOA, MSOA and LAD. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)   
- `london-2011-lsoa-simple.csv` - as for `london-2011-lsoa.shp` but with simplified polygons for smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)  
- `london-2011-lsoa-trunc.csv` - as for `london-2011-lsoa-simple.csv` but with integer co-ordinates for even smaller file size. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb)

> Source: Office for National Statistics licensed under the Open Government Licence v.3.0  
Contains OS data © Crown copyright and database right (2022)

## Population
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/population) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-population-midyear-estimates.ipynb) as follows:
- `london-mid2020-pop.csv` - LSOA mid-year population estimates for 2020.
- `london-mid2019-pop.csv` - LSOA mid-year population estimates for 2019.

>Source: Office for National Statistics licensed under the Open Government Licence.

## Energy
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/energy) as follows:
- `london-2010-2020-gas.csv` - LSOA domestic gas consumption for 2010-2020. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-energy-2010-2020.ipynb)
- `london-2010-2020-elec.csv` - LSOA domestic electricity consumption for 2010-2020. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-energy-2010-2020.ipynb)

>Source: Department for Business, Energy & Industrial Strategy

## Crime
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/crime) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-crime-2011-2020.ipynb) as follows:
- `london-2011-2021-major-arson` - LSOA annual Arson and Criminal Damage crimes (major category)
- `london-2011-2021-major-burglary` - LSOA annual Burglary crimes (major category)
- `london-2011-2021-major-drugs` - LSOA annual Drug Offences crimes (major category)
- `london-2011-2021-major-misc` - LSOA annual Miscellaneous Crimes Against Society crimes (major category)
- `london-2011-2021-major-weapons` - LSOA annual Possession of Weapons crimes (major category)
- `london-2011-2021-major-public-order` - LSOA annual Public Order Offences crimes (major category)
- `london-2011-2021-major-robbery` - LSOA annual Robbery crimes (major category)
- `london-2011-2021-major-sexual` - LSOA annual Sexual Offences crimes (major category)
- `london-2011-2021-major-theft-all` - LSOA annual Theft (non-vehicle) crimes (major category)
- `london-2011-2021-major-vehicle-offences` - LSOA annual Vehicle Offences crimes (major category)
- `london-2011-2021-major-violence` - LSOA annual Violence Against the Person crimes (major category)
- `london-2011-2021-minor-theft-bicycle` - LSOA annual Bicycle Theft crimes (minor category)
- `london-2011-2021-minor-theft-vehicle` - LSOA annual Theft or Taking of a Motor Vehicle crimes (minor category)

> Source: [Metropolitan Police Service](https://data.london.gov.uk/dataset/recorded_crime_summary) licensed under the [Open Government Licence v.2.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/)  
