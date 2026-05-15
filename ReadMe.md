# Read Me
## Delta Research Project
#### Project Contacts: jeff@sierrastreamsinstitute.org, helen@sierrastreamsinstitute.org
#### Updated: 13 May 2026 by Jessica Herrmann

## I. Overview
This repo contains open-source environmental and biological datasets curated by SSI staff for analysis in the Delta Research Project.

Citations for individual datasets can be found under the individual ReadMe markdown files within each separate data folder. Private and/or unpublished data has not been included in this repository.

For more information on data useage, please contact Jeff Lauder or Helen Fitanides (contacts in header).

## II. Project Dataset Folders
### BMI Data
Benthic macroinvertebrate data from SSI's field sites (2025 – 2026), including: sample data including date, location, counts, and taxonomic identification

### Water Quality Data
Water quality datasets both from SSI and partners and from public repositories (California Environmental Data Exchange Network [CEDEN]), including pH, turbidity, dissolved oxygen, conductivity, nutrient loading, bacteria.

### NLCD Data
National Land Cover Database (NLCD) land cover and land cover change spatial data procured from the Multi-Resolution Land Use Consortium MRLC, to be clipped to 1-km and 5-km radius buffers around each site with biological data. 

### Landsat NDVI and P-ET
30-m Landsat Normalized Vegetation Difference Index (NDVI) data, accessed through Google Earth Engine. A reducer function was applied to obtain mean NDVI for each site coordinate point within both a 1-km and 5-km radius buffer. This dataset was also used to calculate Precipitation-Evapotranspiration (P-ET), a climate metric that can in some instances be used as a proxy for surface water runoff.

### TNC Modeled Streamflow Data
Monthly modeled flow data from The Nature Conservancy’s (TNC) Natural Flows Database

### PRISM Climate Data
Parameter-elevation Regressions on Independent Slopes Model (PRISM) daily 800-m gridded climate data, including air temperature, precipitation, vapor pressure deficit (VPD), dew point temperature, and surface solar radiation.

### Estimated Streamflow
SSI’s modeled stream discharge datasets. This folder also included the MS Excel sheet and R script used for deriving estimated streamflow from measurements of channel morphology and water level data.

## III.Example Scripts and Datasets
Please refer to this folder for example NMDS and SEM scripts, as well as the example biological and environmental datasets required to run them.



