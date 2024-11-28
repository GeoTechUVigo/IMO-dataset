# Creation of dataset of intertidal macroalgae (IMO-dataset)

Created by [Andrea Martínez Movilla](https://orcid.org/0000-0002-6114-9074), [Juan Luis Rodriguez Somoza](https://orcid.org/0000-0003-4031-762X and [Joaquín Martínez Sánchez](https://orcid.org/0000-0003-0320-4191) from [GeoTech group](https://geotech.webs.uvigo.es/en/), [Cintex](https://cintecx.uvigo.es/gl/), [UVigo](https://www.uvigo.gal/). 

## Overview
This repository contains the code used in the article 'Dataset of high resolution images of Intertidal Macroalgae'. 

It consists of two scripts:  

The first script (**from_orthoimage_to_labels**) creates a dataset of png images for macroalgae classification. It separates an orthoimage into individual manual labels and saves them as squared images by adding a bounding box of zeros arround them. Each of the images is named by a common filename, the time stamp and the class it represents. 

This script needs as input variables the orthoimage and the manual labels as tif files, the path of the output folder and the common filename for the images created. 

The second script (**CNN_with_labels_example**) uses that dataset to train a convolutional neural network. It needs the path of the folders containing the training and test data. 

## Data

The dataset created with this repository can be found in [Zenodo](https://zenodo.org/records/14185867). If you use it, please cite it as: 

 Martinez-Movilla, A. (2024) «Dataset of high resolution images of Intertidal MacrOalgae (IMO Dataset)». Zenodo. doi: 10.5281/zenodo.14185867.
## Requirements

The code runs in Python 3.9. The required libraries can be installed using the file 'requirements.txt'. The main libraries used are:

- Open cv
- Scikit image
- Scikit learn
- Matplotlib
- Pandas
- Numpy
- Tensorflow
- PIL

## Aknowledgements 

This work was supported by the Galicia Marine Science programme, which is part of Complementary Science Plans for Marine Science of Ministerio de Ciencia e Innovación included in the Recovery, Transformation and Resilience Plan (PRTR-C17.I1), funded through Xunta de Galicia with NextGenerationEU and the European Maritime Fisheries and Aquaculture Funds.

## License 
Copyright (C) 2024 GeoTECH Group geotech@uvigo.gal

Copyright (C) 2024 Andrea Martínez Movilla andrea.martinez.movilla@uvigo.gal

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program in LICENSE. If not, see https://www.gnu.org/licenses/.
