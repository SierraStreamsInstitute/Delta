# Read Me
#### Estimated Streamflow Data For SSI’s Gaged Sites
#### Author: Jessica Herrmann
#### Updated: 13 May 2026

## I. Exccel Workbook and R Script
### Channel Geom Calculator 2.0.xlsx
This is an MS Excel spreadsheet of the modeled channel geometry regression models for each of the fourteen gaged Delta sites.

### QCalculator2_Updated13May2026.Rmd
R Markdown script for calculating estimated streamflow by site, using the site-specific formulas for channel wetted perimeter and cross-sectional area derived in the Channel Geom Calculator 2.0.xlsx document. The input data for this script will be your stage data, with the barometric compensation already completed in HOBOware. The script is currently set up with an example of how to calculate streamflow for Cat Creek. Please note that, at this point, the script is currently set up to run with (commented out) facsimile data, which is intended to be an example. There are placeholder object names set up to run the script with real data.

## II. ERA5 Barometric Pressure Datasets
Since some of our stream gages (SHADY, DC10, DC20, BR55, MON, and EFAR) were not paired with matching HOBO barometric pressure transducers because there are nearby weather stations with atmospheric pressure data already available. Originally, we were planning to use airport baro pressure data from NOAA in order to compensate the raw stage/water pressure files for barometric pressure, however, we will be using the following datasets instead:

### ERA5 Modeled Baro Pressure Datasets
These files are the correct ones to use for performing barometric compensation on our stage datasets for the aforementioned sites. This data is modeled to the resolution of 0.25º x 0.25º grid cells, so site coordinates were approximated to the nearest 0.25º in order to obtain matching surface pressure datasets.  Please note that since sites SHADY and DC20 were close enough to one another to fit within the same grid cell, the same barometric pressure dataset is to be used for both. The files are saved as .csv zip files under SSI's project Drive data folder. They will need to be updated to include data from mid-March through mid-September, 2026, later in the fall of 2026.

## III. Reference
Copernicus Climate Change Service (2025): ERA5 hourly time-series data on single levels from 1940 to present. Copernicus Climate Change Service (C3S) Climate Data Store (CDS). URL: https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels-timeseries (Accessed on 17-03-2026)

Other credits: Bruce Medhurst (SNARL), Dave Herbst (SNARL, SSI), and Poyom Riles (SSI) also contributed significantly to the development of SSI’s methods for estimating streamflow using stage data and channel geometry.
