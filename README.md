# London Data
Spatial data for London, curated for analysis using [ONS geographies](https://www.ons.gov.uk/methodology/geography/ukgeographies). Python code used to manipulate data from original sources is [provided](https://github.com/jamesdamillington/london-data/tree/main/code) (along with a [file](https://github.com/jamesdamillington/london-data/blob/main/code/environment.yml) specifying package requirements).

## Geographies
Boundary data for various geographies the UK ONS uses to produce statistics (e.g. census, electoral). Provided in `.shp` and `.csv` format, usually with [BNG CRS](https://epsg.io/27700).

### Census
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/geographies/census) as follows:
- `london-2021-lsoa-gen20.shp` - LSOA boundaries (generalised to 20m resolution from ONS) for 2021 with codes and names for LSOA, MSOA and LAD.
- `london-2021-lsoa-gen20.csv` - as for `london-2021-lsoa-gen20.shp` but csv format ready to work in geopandas (_this is what most King's students will want to currently work with_).
- `london-2021-lsoa.shp` - LSOA boundaries (original full resolution from ONS) for 2021 with codes and names for LSOA, MSOA and LAD.
- `london-2021-lsoa-simple.csv` - as for `london-2021-lsoa.shp` but with simplified polygons for smaller file size and csv format ready to work in geopandas.
- `london-2021-lsoa-trunc.csv` - as for `london-2021-lsoa-simple.csv` but with integer co-ordinates for even smaller file size and csv format ready to work in geopandas.
- `london-2011-lsoa-gen20.shp` - LSOA boundaries (generalised to 20m resolution from ONS) for 2011 with codes and names for LSOA, MSOA and LAD.
- `london-2011-lsoa-gen20.csv` - as for `london-2011-lsoa-gen20.shp` but csv format ready to work in geopandas.
- `london-2011-lsoa.shp` - LSOA boundaries (original from ONS) for 2011 with codes and names for LSOA, MSOA and LAD.
- `london-2011-lsoa-simple.csv` - as for `london-2011-lsoa.shp` but with simplified polygons for smaller file size and csv format ready to work in geopandas.  
- `london-2011-lsoa-trunc.csv` - as for `london-2011-lsoa-simple.csv` but with integer co-ordinates for even smaller file size and csv format ready to work in geopandas.

Source code for [2021 files](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2021-geography.ipynb) and for [2011 files ](https://github.com/jamesdamillington/london-data/blob/main/code/london-census2011-geography.ipynb).
> Source: Office for National Statistics licensed under the [Open Government Licence v.3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)  
Contains OS data © Crown copyright and database right (2022)

### Roads
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/geographies/roads) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-roads.ipynb) as follows:
- london-2018-MRN.shp - [Major Road Network](https://www.data.gov.uk/dataset/95f58bfa-13d6-4657-9d6f-020589498cfd/major-road-network) clipped to extent of London Boroughs
- london-2023-oproad-MandA.shp - Motorways and A Roads from the [OS Open Roads](https://www.ordnancesurvey.co.uk/products/os-open-roads) data clipped to extent of London Boroughs

> Sources: Department for Transport (2022) licensed under the Open Government Licence v.3.0; Ordnance Survey (OS) licensed under the Open Government Licence v.3.0, Contains OS data © Crown Copyright [and database right] (2023)
 
## Population
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/population) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-population-midyear-estimates.ipynb) as follows:
- `london-mid2020-pop.csv` - LSOA mid-year population estimates for 2020.
- `london-mid2019-pop.csv` - LSOA mid-year population estimates for 2019.

>Source: Office for National Statistics licensed under the [Open Government Licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/1/open-government-licence.htm).

Note: joining these data to 2011 census geographies is not entirely appropriate (e.g. see issue in the [source code notebook](https://github.com/jamesdamillington/london-data/blob/main/code/london-population-midyear-estimates.ipynb))

## Energy
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/energy) as follows:
- `london-2010-2020-gas.csv` - LSOA domestic gas consumption for 2010-2020. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-energy-2010-2020.ipynb)
- `london-2010-2020-elec.csv` - LSOA domestic electricity consumption for 2010-2020. [[Source Code]](https://github.com/jamesdamillington/london-data/blob/main/code/london-energy-2010-2020.ipynb)

>Source: Department for Business, Energy & Industrial Strategy

## Crime
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/crime) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-crime-2011-2020.ipynb) contain annual counts per LOSA as follows:
- `london-2011-2021-major-arson` - Arson and Criminal Damage crimes (major category)
- `london-2011-2021-major-burglary` - Burglary crimes (major category)
- `london-2011-2021-major-drugs` - Drug Offences crimes (major category)
- `london-2011-2021-major-misc` - Miscellaneous Crimes Against Society crimes (major category)
- `london-2011-2021-major-weapons` - Possession of Weapons crimes (major category)
- `london-2011-2021-major-public-order` - Public Order Offences crimes (major category)
- `london-2011-2021-major-robbery` - Robbery crimes (major category)
- `london-2011-2021-major-sexual` - Sexual Offences crimes (major category)
- `london-2011-2021-major-theft-all` - Theft (non-vehicle) crimes (major category)
- `london-2011-2021-major-vehicle-offences` - Vehicle Offences crimes (major category)
- `london-2011-2021-major-violence` - Violence Against the Person crimes (major category)
- `london-2011-2021-minor-theft-bicycle` - Bicycle Theft crimes (minor category)
- `london-2011-2021-minor-theft-vehicle` - Theft or Taking of a Motor Vehicle crimes (minor category)

> Source: [Metropolitan Police Service](https://data.london.gov.uk/dataset/recorded_crime_summary) licensed under the [Open Government Licence v.2.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/)  

## Air Quality
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/airquality) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-airquality.ipynb) are modelled ground level concentrations of pollution summarised for LSOAs from 20m grid resolution data (££ is data geography year '11 or '21, and #### is AQ data collection year 2019, 2016 or 2013):
- `london££-####-PM25` - annual mean PM2.5 (microgramme per cubic metre)  
- `london££-####-PM10` - annual mean PM10 (microgramme per cubic metre)  
- `london££-####-PM10d` - number times daily mean PM10 exceeded 50 microgramme per cubic metre
- `london££-####-NOx` - annual mean NOx (microgramme per cubic metre)
- `london££-####-NO2` - annual mean NO2 (microgramme per cubic metre)

> Source: [London Atmospheric Emissions Inventory (LAEI)](https://data.london.gov.uk/air-quality/) licensed under the [Open Government Licence v.2.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/)  

## Household Income
Data files [here](https://github.com/jamesdamillington/london-data/tree/main/data/economic) from [source code](https://github.com/jamesdamillington/london-data/blob/main/code/london-hhold-income-2001-2012.ipynb) are modelled household income estimates for small areas, London, 2001-2012:
- `london-2001-2012-HHI-mean.csv` - mean total gross household income for LSOAs (2011 geography)
- `london-2001-2012-HHI-median.csv` - median total gross household income for LSOAs (2011 geography)

> Source: [Greater London Authority](https://data.london.gov.uk/dataset/household-income-estimates-small-areas) licensed under the [Open Government Licence v.2.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/)  
