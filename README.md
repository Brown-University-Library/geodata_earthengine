# Using Google Earth Engine with Colab

Google Earth Engine is a planetary-scale platform for satellite imagery and related datasets, available at no cost for academic and personal use. The most commonly used datasets includes satellite imagery from the LANDSAT, SENTINEL, and MODIS programs. However, there are hundreds of other geospatial datasets accessible, including atmospheric, weather and climate data, geological classifications, vegetation indices, and DEMs.

While Earth Engine provides an invaluable source of data, it can be difficult to integrate the custom Javascript editor into the research process. This tutorial uses the Python Google Earth Engine API in conjunction with Google Colab, an online code editor that makes it easy to create and share notebooks. 

**To use this tutorial, download `Using_Google_Earth_Engine_with_Colab.ipynb`. Then, go to Google Colab (colab.research.google.com) and upload the Jupyter notebook.**

This repository contains a Jupyter Notebook for working with Google Earth Engine's Python API in Google Colab. The tutorial uses [USGS Landsat 8 Collection 2 Tier 1 TOA Reflectance data](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_TOA). These LANDSAT images have not been atmospherically corrected. This means that the optical bands have not been scaled and offset, making it easier to work with. The tutorial also chooses to forego QA masking to remove cloud and cloud shadow components. This was deemed unnecessary as cloud NDVI values are typically very low and do not approach the actual vegetation index.

[Google Earth Engine dataset: LANDSAT/LC08/C02/T1_L2](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_L2#description)

[USGS L8 User's Handbook](https://d9-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/atoms/files/LSDS-1574_L8_Data_Users_Handbook-v5.0.pdf).


