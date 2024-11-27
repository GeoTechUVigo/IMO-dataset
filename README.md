# Creation of dataset of intertidal macroalgae (IMO-dataset)
Created by [Andrea Martínez Movilla](https://orcid.org/0000-0002-6114-9074) from [GeoTech group](https://geotech.webs.uvigo.es/en/), [Cintex](https://cintecx.uvigo.es/gl/), [UVigo](https://www.uvigo.gal/). 

## Overview
This repository contains the code used in the article 'Dataset of high resolution images of Intertidal Macroalgae'. 

It consists of two scripts:  

The first script creates a dataset of png images for macroalgae classification. It separates an orthoimage into individual manual labels and saves them as squared images by adding a bounding box of zeros arround them. Each of the images is named by a common filename, the time stamp and the class it represents. 

This script needs as input variables the orthoimage and the manual labels as tif files, the path of the output folder and the common filename for the images created. 

The second script uses that dataset to train a convolutional neural network. It needs the path of the folders containing the training and test data. 

## Data
The dataset created with this repository can be found in [Zenodo](https://zenodo.org/records/14185867). If you use it, please cite it as: 

 Martinez-Movilla, A. (2024) «Dataset of high resolution images of Intertidal MacrOalgae (IMO Dataset)». Zenodo. doi: 10.5281/zenodo.14185867.
## Requirements
The code runs in Python. The required libraries can be installed using the file 'requirements.txt'. The main libraries used are:

- Open cv
- Scikit image
- Scikit learn
- Matplotlib
- Pandas
- Numpy
- Tensorflow
- PIL

## License 

Automated instance and semantic segmentation of point clouds of large metallic truss bridges.

Copyright (C) 2024 GeoTECH Group geotech@uvigo.gal

Copyright (C) 2024 Andrea Martínez-Movilla andrea.martinez.movilla@uvigo.gal


This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program in LICENSE. If not, see https://www.gnu.org/licenses/.
