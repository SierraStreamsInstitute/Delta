# Read Me
#### Annual MRLC NLCD Data
#### Author: Jessica Herrmann
#### Updated: 13 May 2026

## I. Background
This folder contains annual MRLC land cover data for each of SSI's field and supplemental sites. Each land cover class has been calculated as a percentage out of total pixel count within both 1- and 5-km geodesic buffered regions around each site point.

Note that, for the purposes of this study, we only evaluated land cover within the bounds of the Huc8 watersheds referenced in the DeltaHuc8_20260323.zip file described below. So for a few of the sites, the 5-km buffers extended beyond the extent of the NLCD rasters, and therefore, the total pixel count was lower for these buffers.

For additional scripts, source datasets, and access to the ArcGIS project file, please contact SSI (jeff@sierrastreamsinstitute.org).

## II. Huc8 Shapefile
### DeltaHuc8_20260322.zip
Merged Huc8 shapefile of all Delta project watersheds, created by Melissa Grim, 2026

## III. 2004 – 2024 NLCD Dataset
### Delta_NLCDpct_1km_5km_2004_2024.csv 
This is the edited NLCD dataset to be used for analysis, until 2026 data becomes available.

Land cover class codes were converted to brief descriptions of cover type and organized as column headers. Each LC class column has either a “.1km” or “.5km” qualifier, indicating the spatial extent of the buffer region around each site point. In addition, the “.pct” qualifier indicates that each LC column gives the percentage of pixels out of total pixel count within the buffer, per LC class and buffer area. I organized the data this way so that it would be easier to use for NMDS later on.

IMPORTANT – Please keep in mind that, due to periodic (annual?) algorithm changes that affect MRCL’s land cover classifications, these datasets will need to be entirely re-pulled, and any prior analyses will have to be re-run, if you are updating the dataset in the future (e.g. in 2027, when pulling data for 2025 onward). Please treat each data pull as an entirely new dataset; i.e. you cannot simply add the data from 2025 to the existing data in the Google Drive or GitHub, as it may not be completely comparable. Instead, in order to accurately update this dataset, you will need to re-download all data from 2005 through the most recent year available.

## IV. Reference
U.S. Geological Survey (USGS), 2024, Annual NLCD Collection 1 Science Products: U.S. Geological Survey data release, https://doi.org/10.5066/P94UXNTS
