# Read Me
#### Landsat NDVI Data & P-ET
#### Author: Jessica Herrmann
#### Updated: 13 May 2026

## I. Background & Data Sources
This folder contains scripts and finalized datasets for Landsat NDVI and derived precipitation minus evapotranspiration (P-ET). I have pulled NDVI data from the Landsat 30-m 8-day composite dataset and used a reducer function to obtain mean NDVI for each site coordinate point within both a 1-km and 5-km radius buffer. The “composite” refers to a composite of all scenes within an 8-day period. This data is available per 8-day increment, when scenes are available, so there will be gaps in the data when no scenes are available within a given 8-day period or when there are issues with cloud cover or data quality. I chose this dataset because it is the most recent continuous, single-source dataset I could find for near-daily NDVI data for our reference period of 2005 – 2025+, unless we were to cobble together more recent Landsat data and the older Sentinel datasets.

This folder also contains a P-ET dataset for all sites, for water years 2006 through 2024. Since we do not yet have the full, stable PRISM precipitation data from 2025 (as of April 2026), we cannot yet calculate P-ET for WY 2025.

## II. Datasets
### ALLDeltaSitesLandsat8DayNDVI_1KM_5KM_2005_2025.csv
– This file contains NDVI data for all field and supplemental sites combined. The “meanNDVI_1km” and “meanNDVI_5km” columns specify the spatial buffers used to calculate mean NDVI by site. All data for calendar years 2005 through 2025.

### Delta_P_ET_WY2006_2024.csv
– File containing calculated P-ET for hydrological years 2006 through 2024. Since NDVI was originally calculated as the mean within 1-km and 5-km buffers, there are two P-ET calculations, one for each respective spatial buffer.

## III. GEE JavaScript
### Delta Landsat NDVI Annotated JavaScript
– A text document JavaScript set up to download NDVI data for the sites we will be referencing for biological/BMI data: all field sites surveyed by SSI for the Delta Project, as well as all supplemental sites (CEDEN and SYRCL). You can copy and paste this script into the Google Earth Engine code editor and update the highlighted values to download more data. To pull additional data, you will only need to change the date range and output file names in order to download the mean NDVI data for 2026 and beyond.

### DeltaFieldSiteCoords.csv and DeltaSuppSiteCoords.csv
– Locations files formatted for compatibility with GEE’s code editor. Just upload these files to the “Assets” tab in the GEE code editor, and specify the document’s column names for the latitude and longitude fields (should be “Lat” and “Long”), in order to extract more data for all sites. Alternatively, you can modify these location files using the Delta Site Coords for GEE sheet, then re-download one or both tabs as CSV files and upload to GEE.

## IV. P-ET R Script
### Delta_PET_updatedApr2026.Rmd
– This Rmd script calculates P-ET for all field and supplemental sites, from water years 2006 through 2024. P-ET may potentially be used as a proxy for groundwater runoff (Rungee et al. 2021). Please refer to the P-ET sub-folder under the Delta Research project Papers folder for more background information on the method. I used the daily 800-m precip data and calculated the total annual precipitation for each water year, then took the two-water year average in order to calculate PP. I also used 30-m 8-day NDVI data to calculate evapotranspiration (ET). Since there are gaps in the NDVI dataset, and Rungee model calls for mean NDVI by year/water year, I calculated average NDVI by site and water year and just excluded any NA values in the average calculations.

## V. References
PRISM Group, Oregon State University, https://prism.oregonstate.edu, accessed 7 Apr. 2026.

Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey.
