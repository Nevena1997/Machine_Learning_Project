# ML Project
## Face Mask Detector

**Authors:** Nađa Obrenović, Nevena Vilotić

**Language:** Python

**Requirements:** [requirements.txt]()

## About the project
The idea of the project is the construction of a Face Mask Detector that would, for all detected faces in the image, determine whether there is a mask on them or not.
Face Mask Detector is a model which is based on computer vision and deep learning. It can be integrated with computer or laptop cameras. 

The above idea is implemented through the following stages. At the first stage, all the faces in the image are detected by cascade classifier, which determines the region of interest. Afterwards, the region of face is extracted, resized to 100x100 and passed to convolutional neural network, which gives a probability of presence of the mask. In the next stage, all previously detected faces are framed and contain a simple message e.g. 'MASK' nad 'NO MASK', depending on results of the model. The message is also followed by a probability that its statement is true.  

![](https://user-images.githubusercontent.com/74012107/130773556-28eb52f0-e368-4506-82eb-75a564754664.png)




## Dataset
The dataset used in this project is available at [Kaggle](https://www.kaggle.com/ashishjangra27/face-mask-12k-images-dataset).
It consists of with mask and without mask images:
- *Train dataset* with 10 000 images (5000 face images with masks and 5000 without masks)  
- *Validation dataset* with 800 images (400 face images with masks and 400 without masks)
- *Test dataset* with 992 images (483 face images with masks and 509 without masks).

## Literature
[COVID-19 Face Mask Detection](https://www.dpublication.com/wp-content/uploads/2021/03/28-418.pdf)

[Detect Face-Masks for COVID-19](https://www.mdpi.com/2076-3417/11/5/2070)
