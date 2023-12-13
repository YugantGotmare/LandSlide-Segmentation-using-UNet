# LandSlide-Segmentation-using-UNet

# Project Name

Landslide Segmentation using UNet

## Description

This project focuses on implementing a landslide segmentation model using the UNet architecture. The model is trained on satellite images with associated masks to identify regions prone to landslides. It includes preprocessing steps, model training, and the ability to make predictions on new data.

## Data Description

The Landslide4Sense dataset has three splits, training/validation/test, consisting of 3799, 245, and 800 image patches, respectively. Each image patch is a composite of 14 bands that include:

- **Multispectral data** from [Sentinel-2](https://sentinel.esa.int/web/sentinel/missions/sentinel-2): B1, B2, B3, B4, B5, B6, B7, B8, B9, B10, B11, B12.

- **Slope data** from [ALOS PALSAR](https://www.usgs.gov/centers/eros/science/usgs-eros-archive-radar-alos-palsar-radar-processing-system): B13.

- **Digital elevation model (DEM)** from [ALOS PALSAR](https://www.usgs.gov/centers/eros/science/usgs-eros-archive-radar-alos-palsar-radar-processing-system): B14.

All bands in the competition dataset are resized to the resolution of ~10m per pixel. The image patches have the size of 128 x 128 pixels and are labeled pixel-wise.

data link:- https://www.kaggle.com/datasets/pypiahmad/landslide4sense-challenge

## UNet Architecture

This project leverages the UNet architecture, a convolutional neural network (CNN) designed for image segmentation tasks. UNet is particularly well-suited for biomedical image segmentation but has found applications in various domains. The architecture consists of a contracting path to capture context and a symmetric expanding path to enable precise localization. Its distinctive U-shape structure allows the model to maintain fine spatial information during the encoding and decoding stages, making it effective for tasks like landslide segmentation. The use of skip connections facilitates the fusion of high-level features with detailed spatial information, contributing to accurate segmentation results.


## Prerequisites

- Python 3.x
- TensorFlow 2.x
- h5py
- NumPy
- Matplotlib
- OpenCV (cv2)

## Training Progress
![graph](https://github.com/YugantGotmare/LandSlide-Segmentation-using-UNet/assets/101650315/abe467b0-b917-40b8-bb23-0039c0c42fb3)

## Result



![result_1](https://github.com/YugantGotmare/LandSlide-Segmentation-using-UNet/assets/101650315/2eec690d-470b-4a40-a687-f39a2dcbc457)



