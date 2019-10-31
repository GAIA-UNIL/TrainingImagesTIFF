# TrainingImagesTIFF
Tiff version of various training images used in the literature. Useful for direct used in example codes.
Image converted form [this repository](https://github.com/GAIA-UNIL/trainingimages)

## To load training images in Matlab

```
ti=imread('https://raw.githubusercontent.com/GAIA-UNIL/TrainingImagesTIFF/master/{fileName.tiff}')
``` 
Remplacing ```{fileName.tiff}``` with the file of interest. 

## To load training images in Python3

```
import numpy
from PIL import Image
import requests
from io import BytesIO

ti = numpy.array(Image.open(BytesIO(requests.get('https://raw.githubusercontent.com/GAIA-UNIL/TrainingImagesTIFF/master/{fileName.tiff}').content)));
```
Remplacing ```{fileName.tiff}``` with the file of interest.