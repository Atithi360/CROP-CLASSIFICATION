# CROP CLASSIFCATION MODEL
## _Mini Project Course 2021 SEM - V_
Under the supervision of **Dr. Triloki Pant** 

Team Members
- Devang Bharti(IIB2019020) 
- Ritu Kiran Murmu(IIB2019025)
- Atithi Kumari(IIB2019026) 
- Anajali Kumari(IIB2019037)

## Problem Statement
Process Landsat-8 and Sentinel-2 images with the help of some image fusion method for crop classification. You may apply PCA, IHS model or deep learning model (or any other of your choice) for fusion of high resolution images (10m and 30m for example). Once a fused image is at hand, try to classify it for various crops and extract the crop details accurately. 
You may choose any open source tool like QGIS for visualizing the images and any programming for the processing of data.
Use the following study area: Prayagraj with corner points: (25˚31ˊ21.55˝N, 81˚39ˊ17.30˝E) and (25˚17ˊ22.08˝N, 81˚57ˊ39.17˝E).

## Description
This repository implements multispectral images fusion algorithms based on the wavelet transform. The fused images along with ground-truths value for the top 6 crop yields were digitized and labeled with the help of ArcGIS tools. Then the labeled crop images were preprocessed for NDVI classification and classification model. We have used Sequential Deep learning Models for classification of our data. 

We modelled two Deep Learning models: -
- Accuracy of 1st one: - **81.22%**
- Accuracy of 2nd one: - **95.02%**


The landasat 8 and sentinel 2 images used are downloaded from [USGS](https://earthexplorer.usgs.gov/).

## Installation
We can use google colab to execute the jupyter notebook files.
## Usage
There are 2 main execution flows: -

-   Multispectral images fusion: To perform multispectral images fusion, run [resizing.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/resizing.ipynb) to       resize the Landsat 8 image to the Sentinel 2 image pixel size. Finally, we can do the           multispectral images fusion by executing [image_fusion.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/image_fusion.ipynb) .
-   Then we are digitizing area of crop fields to the provided Lat/Lon of the ground-truth locations along with labelling with the help of arcGIS tools.
-   Crop classification model: The labled crop images are preprocessed for NDVI based classification and crop classification model. These are executed in [classification_model_1.ipynb](https://github.com/Atithi360/CROP-CLASSIFICATION/blob/main/Crop%20Classification/classification_model_1.ipynb).

## Dataset
Fused images after fusion of Landsat8 and sentinel 2 can be accessed from [here](https://drive.google.com/drive/folders/1lP-MDHepi_2Ia0KuAO7M-xhMD7bpURnt?usp=sharing).

After digitizing and labelling, the labeled crop dataset for classification is uploaded [here](https://drive.google.com/drive/folders/15Nm385ouzdO9wZJO6pwCvWnY0thUGtjK?usp=sharing).

## Tech

We used these tech stacks:
-   [ArcGIS](https://www.arcgis.com)  - cloud-based mapping and analysis solution

-   [google colab](https://colab.research.google.com/#create=true) - to write and execute arbitrary python code through the browser
-   [python](https://www.python.org) 
