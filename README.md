# Cataract-Eye-Disease-Detection

## Libraries used:- Matplotlib, Seaborn, Sci-Kit Learn, Tensorflow, PIL, OpenCV etc.

This repository contains some of the notebooks which I used for building a Covolutional Neural Network for the binary classification of normal eye images and cataract eyes. The novelty of the work is that, it is for the first time eye images captured from digital cameras are directly used for cataract identification. 

## Abstract:-
Early detection of cataract plays a vital role in ensuring prevention of vision loss. This paper aims to propose an algorithm that will act as an assistive measure in the process of automating cataract disease detection. Majority of the existing works are focussed on the utilization of either fundus images or visible wavelength images captured using DSLR camera individually. The novelty of this proposed algorithm is the capability to deliver equally accurate and precise performance using both normally captured visible wavelength images as well as medically captured anterior segment images which can in turn prove to be cost effective as well. The image pre-processing techniques particularly adaptive thresholding hereby employed provides fast and accurate results on the input dataset fed to the CNN model which in turn is a fine-tuned version of Inception-v3. Here the training of the model has been done using visible wavelength images whereas the validation testing has been done using the anterior segment eye images medically obtained from a hospital. The proposed image pre-processing technique along with the model architecture ensures the achievement of high classification accuracy
of about 95%. Since the model deals with examination of the anterior segment of the image, cases concerning nuclear cataract, cortical cataract or a hybrid case involving the detection of both the aforementioned cataract types lie under the range of detection of our system.

## Dataset Details:- 
A mixture of visible wavelength eye images are used, around 2508 images were used for training consisting of 1254 images of both classes. While 568 images were used for validation with 284 images belonging to each category. The entire dataset was split in the ratio of 81.5:18.5. Apart from this "3netra classic" data collected from Korade Eye Hospital, Nashik with due consent of patients is used for testing.
* The images are collected from online sources as well as from Eye Clinics. Because of privacy concerns the data is not publicised.

## Classes:- 
Normal Eye, Cataract Eye

Images were found to have different types of noise and distortions, hence image processing techniques were applied for the precise classification task.
Some of them are:-
1) Morphological Dilation is used to remove specular reflection
2) Canny Edge Detection, Hough Circle Detection 
3) Histogram Analysis 
4) Hough transformation
5) Adaptive Thresholding

## Image Size:- 
224 * 224 * 3 (RGB)

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

## Validation Accuracy(In the notebook given):- 
93.66%

## 5-Fold Cross Validation Results
* Mean Accuracy = 99.84%
* Standard Deviation = 0.3187
* Variance = 0.0010159
