# Deep-Learning-assisted-Diagnosis-for-knee-injuries
Implementation of a convolutional neural network that classifies ACL tears from MRI exams

## Dataset
The data comes from Stanford ML Group research lab. It consits of 1,370 knee MRI exams performed at Stanford University Medical Center to 
study the presence of Anterior Cruciate Ligament (ACL) tears.

## Code Structure

### model.py
* Defines model's architecture
* Performs transfer learing by loading pretrained CNN model. 

### dataloader.py
* Loads the data and apply data augmentation

### train.py
* It imports dataloader.py to load the data from both train or validation sets.
* It imports model.py and instantiates an MRNet model before updating its weights.
* It launches a training and validation loop over a given number of epochs.

## Results
I trained an ACL tear classifier on a sagittal plane and got the following AUC scores:

on train: 0.8669\
on validation: 0.8850
