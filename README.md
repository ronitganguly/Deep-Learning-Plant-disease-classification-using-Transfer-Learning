# Deep-Learning-Plant-disease-classification
# The attributions of the data source have been mentioned in the report.
# Highlighted concepts used:
1) Pytorch.
2) Facebook's Adaptive Experimentation for hyper-parameter tuning.
3) K-fold cross validation using Pytorch.
4) Transfer Learning - **Resnet50, VGG16-Batch Normalization version, Alexnet.**
5) Data Visualization.

### Please read the [pdf report](https://github.com/ronitganguly/Deep-Learning-Plant-disease-classification-using-Transfer-Learning/blob/master/Ronit%20Ganguly%202487190G.pdf) to understand about the data or directly check the code where for every cell, a detailed description has been provided. 


## Data Distribution:
--There are 12 classes: 
--Apple Black-rot,
--Apple Healthy,
--Corn Blight,
--Corn Healthy,
--Tomato Blight,
--Tomato Healthy,
--Pepper Bell Bacterial Infection,
--Pepper Healthy,
--Tomato Mould Infection,
--Tomato Spider Mites Infection,
--Flowers (random),
--Cheek Weed (a common crop weed).
--The data is split into training set, validation set and testing set.
--These 3 sets can be found within the folder named "more plant dataset" on colab.
--Training set contains 200 Images per class.
--Both the validation set and the testing set contain 50 images per class.

## Visualization:
![Plant](/Images/Capture1.PNG)

### Some basic inferences and challenges:
--All the images have three channels.
--Flowers should be totally distinguishable from the rest.
--Plants that can be confused with such as tomato healthy, tomato mould, tomato blight, 
tomato spider mites infection because they are the same plants and the data also 
contains initial stages of symptoms which may be indistinguishable by humans. 
--Blight can be confused with pepper bell bacterial infection because the symptoms are 
similar. Hence, this is a challenge for the architecture to properly differentiate between 
these two diseases.
--Since blight and mould can be very similar, tomato mould and tomato blight can be 
mixed with and wrong results can be observed. So, this is a greater challenge for the 
architecture.

## Baseline model

### Training Loss Curve:

![Plant](/Images/Capture2.PNG)

## Resnet50:

### Training Loss curve:

![Plant](/Images/Capture4.PNG)

### Confusion Matrix:

![Plant](/Images/Capture5.PNG)


