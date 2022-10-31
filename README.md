# Cataract-Eye-Disease-Detection

## Libraries used:- Matplotlib, Seaborn, Sci-Kit Learn, Tensorflow, PIL, OpenCV etc.

This repository contains some of the notebooks which I used for building a Covolutional Neural Network for the binary classification of normal eye images and cataract eyes. The novelty of the work is that, it is for the first time eye images captured from digital cameras are directly used for cataract identification. 

## Dataset Details:- 
A mixture of visible wavelength eye images are used, around 2508 images were used for training consisting of 1254 images of both classes. While 568 images were used for validation with 284 images belonging to each category. The entire dataset was split in the ratio of 81.5:18.5. Apart from this "3netra classic" data collected from Korade Eye Hospital, Nashik with due consent of patients is used for testing.
* The images are collected from online sources as well as from Eye Clinics. Because of privacy concerns the data is not publicised.

## Classes:- Normal Eye, Cataract Eye

Images were found to have different types of noise and distortions, hence image processing techniques were applied for the precise classification task.
Some of them are:-
1) Morphological Dilation is used to remove specular reflection
2) Canny Edge Detection, Hough Circle Detection and Cropping the detected circle -> to determine the region of interest(ROI)
3) Histogram Analysis 
4) Hough transformation
5) Adaptive Thresholding

## Image Size:- 224 * 224 * 3 (RGB)

## Deep Neural Network:- 
InceptionV3 (Fine Tuning Technique)

## Type:- 
Binary Classification

## Status:- 
Currently, the journal is under final stage of review with Biomedical and Signal Processing Journal and is due to be published soon.

## Results - Confusion Matrix
![image](https://user-images.githubusercontent.com/106440078/199012781-4c64c4d9-e1d7-415c-b75d-234d37f8d314.png)

* Training Accuracy:- 99% 
* Validation Accuracy:- 95%
* Testing Accuracy:- 94.63%
* Validation Precision:- 99.14% 
* Validation Recall:- 99.30%
* Validation F1-Score:- 99.21%

## Testing Accuracy:- 93.66%(In the notebook given) 

## 5-Fold Cross Validation Results
* Mean Accuracy = 99.84%
* Standard Deviation = 0.3187
* Variance = 0.0010159
