# Using Google Earth Engine with Colab

This repository contains a tutorial for working with Google Earth Engine's Python API in Google Colab. The tutorial uses [USGS Landsat 8 Collection 2 Tier 1 TOA Reflectance data](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_TOA). These LANDSAT images have not been atmospherically corrected. This means that the optical bands have not been scaled and offset, making it easier to work with. The tutorial also chooses to forego QA masking to remove cloud and cloud shadow components. This was deemed unnecessary as cloud NDVI values are typically very low, and do not approach the actual vegetation index.

As a resource to researchers who want to compare NDVI year-to-year without using Google Earth Engine, the repository also contains maximum NDVI composites of Rhode Island in geoTIFF format, derived from [USGS Landsat 8 Level 2, Collection 2, Tier 1](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_L2) surface reflectance data. These are provided for the year and the summer months (June to July), in both cases taking the pixelwise maximum NDVI. For these indices, QA masking was performed to remove saturated pixels and cloud cover, and the optical bands were scaled and adjusted to their original values. The final composites were also clipped to the state extent and with TIGER/LINE boundaries (sourced from the [Ocean State Spatial Database](https://github.com/Brown-University-Library/geodata_ossdb)).

[Google Earth Engine dataset: LANDSAT/LC08/C02/T1_L2](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_L2#description)

[USGS L8 User's Handbook](https://d9-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/atoms/files/LSDS-1574_L8_Data_Users_Handbook-v5.0.pdf).


In the 2019 and 2020 years, the summer composites have significant patches of missing data in the western RI region, likely due to cloud cover or saturation. The yearly composite has less cloud cover, but it is still present in significant areas.

