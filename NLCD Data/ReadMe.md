# Read Me
#### Delta Project – Annual MRLC NLCD Data
#### Author: Jessica Herrmann
#### Updated: 13 May 2026


## I. Huc8 Shapefiles
DeltaHuc8_20260322.zip – Huc8 shapefiles of all Delta project watersheds, created by Melissa Grim, 2026


## II. MRLC Land Cover (LndCov)
NLCD20042024.zip file – zipped folder containing the land cover (LndCov) data, merged for all project Huc8 watersheds and organized by year, from 2004 – 2024. This is the folder I referenced for the analysis in Arc, and this .zip file is also redundantly located under the ArcGIS Project folder for added convenience.

To download additional data, you will need to upload the Huc8 shapefile to the data explorer (“upload shapefile”), and select your datasets and timeline of interest. EPSG3857 is the default CRS for MRLC, but Arc re-projects the TIFF files into WGS84 to match the other input data.

IMPORTANT – Keep in mind that, due to periodic (annual?) algorithm changes that affect MRCL’s land cover classifications, these datasets will need to be entirely re-pulled, and any prior analyses will have to be re-run, if you are updating the dataset in the future (e.g. in 2027, when pulling data for 2025 onward). Please treat each data pull as an entirely new dataset; i.e. you cannot simply add the data from 2025 to the existing data in the Drive, as it may not be completely comparable. Instead, in order to accurately update this dataset, you will need to re-download all data from 2005 through the most recent year available. (We got this tip from Raffi.)

## III. R Script
Delta_NLCDEdit_JHerrmann_2026.Rmd – This is an annotated .Rmd script that reformats the output tables for land cover area and pixel count from ArcGIS.

## IV. ArcGIS Project
DeltaNLCDData.ppkg – ArcGIS project package that takes the annual MRLC NLCD datasets and uses two separate models to iteratively tabulate the area and pixel count of land cover classes within 1- and 5-km geodesic spatial buffers around each SSI field site and supplemental site. Input files to include in the project geodatabase are:

ALLDeltaSites.csv – The site coordinates dataset

NLCD20042024.zip – A zipped folder containing all NLCD geoTIFFs

## V. 2004 – 2024 NLCD Datasets

Delta_NLCDall_1km_5km_2004_2024.csv – This file is the same as the above file, just with raw pixel counts also included as columns.

## Reference
U.S. Geological Survey (USGS), 2024, Annual NLCD Collection 1 Science Products: U.S. Geological Survey data release, https://doi.org/10.5066/P94UXNTS
