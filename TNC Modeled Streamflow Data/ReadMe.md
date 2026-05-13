# Read Me
#### Delta Project TNC Natural Flows Data
#### Author: Jessica Herrmann
#### Updated: 1 Apr. 2026

## I. Background
This folder contains monthly modeled flow data from 2005 through early 2026, from The Nature Conservancy’s Natural Flows Database. Please refer to the SSI Field Site COMIDs document for the COMIDs (common identifiers) of each modeled reach used in this data pull. I selected only one COMID per Delta site, even if there were multiple potential COMIDs to choose from, aiming to select the modeled reach that best overlapped with the majority of our 100-m reaches. The second tab in that document, “Nearby Gages”, is a list of gaged (USGS, CDEC) reaches that are close to, but not perfectly overlapping with, our Delta sites. I’ve also included some notes on the proximity of the gaged reach to the corresponding Delta reach, as well as information on the number of downstream tributaries. Please note that “estimated” flow is modeled unimpaired flow, so it is unlikely to be 100% accurate for heavily-managed systems, though it may be a good approximation for more remote third-order streams, especially if they are close to gaged reaches with observable flows. The CEDEN & SYRCL COMIDs document is a similar list compiled by Melissa Grim for the CEDEN supplemental sites and the one SYRCL site also referenced for BMI data. Some of the sites will share the same COMID. I pulled data from as early as 2005 so as to include the full 2006 water year.

Here are the parameters I have pulled data for:
Statistic: min, mean, median, and max estimated flow (units are cfs)
Variable: specifies if flow data is estimated (modeled) or observed (from a USGS or CDEC gage)

## II. Data Source
This website was used to pull modeled flow data: https://rivers.codefornature.org/#/map. To pull further flow data for the rest of 2026 and beyond, simply copy and paste from the list of COMIDs in the site COMIDs documents, then hit the + sign to add each of the COMIDs to the queue for batch downloading. This will give you estimated (and observed, where available) flows for the modeled reaches that correspond with our field and supplemental sites.

## III. R Script
### TNC Flow Metadata Join.Rmd
– This is a rough .Rmd doc outlining how I reformatted the original datasets from TNC to the final versions under the Datasets folder

## IV. NHD COMIDs by Site
### SSI Field Site COMIDs
– COMIDs for all of SSI’s Delta field sites

### CEDEN & SYRCL Site COMIDs
– COMIDs for CEDEN and SYRCL supplemental sites

## V. Datasets
### Delta_SSIFieldSites_TNCFlowData_2005_2026
– TNC modeled flow data for SSI’s field sites. Some of our sites were close to gaged reaches. I have downloaded this data and saved it as a separate file called Delta_SSIFieldSites_TNCNearbyGagesFlowData_1999_2025.csv. While likely not necessary for building models for the Delta Project, this second dataset may be useful for comparing some of our estimated flow data (as well as TNC modeled flow data) to observed flows at nearby gages.

### Delta_CEDEN_SYRCLSites_TNCFlowData_2005_2026
– TNC modeled flow data for supplemental sites

### Delta_SSIFieldSites_TNCNearbyGagesFlowData_1999_2025
– This is an earlier dataset I pulled that is optional for further analysis but could be useful for comparing our modeled flow data in the 2025 – 2026 SSI Estimated Flow Data folder to data from nearby gages, mainly the Butte Creek site (BUT). Included in this dataset are some of my notes on proximity of the gaged reach to the corresponding Delta reach, as well as information on the number of downstream tributaries.

## VI. Reference
Julie K.H. Zimmerman, Daren M. Carlisle, Jason T. May, Kirk R. Klausmeyer, Theodore E. Grantham, Larry R. Brown, Jeanette K. Howard. California Unimpaired Flows Database v2.1.2, 2023. The Nature Conservancy. San Francisco CA. https://rivers.codefornature.org/ Date Accessed: 1 April 2026.
