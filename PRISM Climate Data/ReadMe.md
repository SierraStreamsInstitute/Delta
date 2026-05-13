# Read Me
#### PRISM Climate Data
#### Author: Jessica Herrmann
#### Updated: 13 May 2026

## I. Background
This folder contains daily 800-m gridded PRISM climate data for each year from 2005 through 2024. All climate parameters are in SI metric units. Since August through December of 2025 (and 2026) are either provisional or not yet available on PRISM’s website, I have only pulled the stable climate data relating to this project so far. I have also concatenated all of the individual yearly files into larger files, one for SSI’s field sites, and one for all supplemental (CEDEN and SYRCL) sites. This website was used to pull daily data from PRISM: https://prism.oregonstate.edu/explorer/bulk.php

Here are the parameters I have pulled data for:
Elevation (m)
Precipitation (mm)
Minimum temperature (ºC)
Maximum temperature (ºC)
Mean temperature (ºC)
Minimum VPD (hPa)
Maximum VPD (hPa)
Mean dewpoint temperature (ºC)
Solar radiation, horizontal surfaces (MJ/m^2/day)
Solar radiation, sloped surfaces (MJ/m^2/day)

## II. Locations Files
### SSI Field Site Locations
Please use this locations file to pull remaining PRISM data for SSI field sites for 2005 – 2026, as it is pre-formatted for compatibility with the PRISM Data Explorer.

### Supplemental Site Locations
Please use this locations file to pull remaining PRISM data for supplemental sites for 2005 – 2026.

## III. Datasets
### DeltaFieldSites_PRISM_2005_2024 and DeltaSupplementalSites_PRISM_2005_2024
Cleaned and concatenated datasets, combined for all years under respective site types (field vs. supplemental). These final datasets should be set up and ready to go for analysis.

## IV. Reference
PRISM Group, Oregon State University, https://prism.oregonstate.edu, accessed 7 Apr. 2026.
