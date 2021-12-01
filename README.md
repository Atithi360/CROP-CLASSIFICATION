# CROP CLASSIFCATION MODEL
## Problem Statement
Process Landsat-8 and Sentinel-2 images with the help of some image fusion method for crop classification. You may apply PCA, IHS model or deep learning model (or any other of your choice) for fusion of high resolution images (10m and 30m for example). Once a fused image is at hand, try to classify it for various crops and extract the crop details accurately. You may choose any open source tool like QGIS for visualizing the images and any programming for the processing of data.
Use the following study area: Prayagraj with corner points: (25˚31ˊ21.55˝N, 81˚39ˊ17.30˝E) and (25˚17ˊ22.08˝N, 81˚57ˊ39.17˝E).

## Description
This repository implements multispectral images fusion algorithms based on the wavelet transform calculated by the à trous algorithm, using Python, which is further used for crop classification. The images used are downloaded from [USGS](https://earthexplorer.usgs.gov/).
The crop information (i.e. ground-truth data) was collected over locations of Prayagraj. We have collected ground-truths value for the top 6 crop yields in the region ex wheat, Paddy,  Bajra, Arhar, mustard, and gram.
## Installation
To execute the jupyter notebooks, an environment including the dependencies is offered. This environment can be found in image_fusion.yml. After importing the environment in conda. You can proceed with the execution of the notebooks.

## Usage
There are 2 main execution flows: -

-   Multispectral images fusion: To perform multispectral images fusion, run [resizing.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/resizing.ipynb) to       resize the Landsat 8 image to the Sentinel 2 image pixel size. Finally, we can do the           multispectral images fusion by executing [image_fusion.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/image_fusion.ipynb) .
-   Then we are digitizing area of crop fields to the provided Lat/Lon of the ground-truth locations with the help of arcGIS tools.
-   Crop classification model: We can execute [classification_model_1.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/classification_model_1.ipynb) to classify our crops.

## Tech

We used these tech stacks:
-   [ArcGIS](https://www.arcgis.com)  - cloud-based mapping and analysis solution

-   [google colab](https://colab.research.google.com/#create=true) - to write and execute arbitrary python code through the browser
-   [python](https://www.python.org) 
