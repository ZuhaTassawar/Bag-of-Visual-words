# Image Feature Detection and Matching Classification

The Bag of Visual Words (BoVW) model is a crucial concept in computer vision for image classification. BoVW is highly scalable and accurate, making it ideal for developing Content-Based Image Retrieval (CBIR) systems. BoVW is also useful for texture classification using textons. This paper aims to explore the underlying principles and techniques of BoVW.


## Introduction
The concept of "Bag of Visual Words" is derived from the concept of "Bag of Words" from the Natural Language Processing Domain. In Bag of Words, the text is represented with it's occurrence frequency without taking into account the order of the words (Hence "Bag" and not list or array). Documents that share a large number of same keywords are considered to be similar or relavant to each other. Treating any textual file or document as a "bag of words" is a more efficient method to compare and analyze becuase the locality of words does not have to be stored and taken to account.

In Computer Vision, the same concept can be applied for images as well. Our "words" are now patched of images along with their feature descriptors. The bag of words model can be utilized in object categorization by creating an extensive vocabulary of visual words and creating a histogram that represents each image's frequency of occurrence of the words in the image. 

In this report, we will be doing Image classification. This will be done in three stages:

    1. Represent each training image by a vector
    2. Train a classifier to discriminate vectors corresponding to positive and negative training images
    3. Apply the trained classifier to the test image

### Methadology Diagram

![Methodology](https://github.com/ZTHussain/Computer-Vision-A1/blob/2fb472558ef40cc3bdf40ca57d275942301ebafc/images/Screenshot%202023-03-13%20070019.png)

## Setup

The setup can be done through one of the following methods:

Create a new conda environment and install the following packages:

    1. Python (conda env)
    2. opencv-Python
    3. scipy
    4. scikit-image
    5. matplotlib
    6. numpy
    7. tqdm
`



## Results

SVM with SIFT on Objects Dataset gives an accuracy of 75\% while on Flower Dataset it gives an accuracy of 30\%.

With ORB and K-Nearest Neighbour as a classifier gave a very poor accuracy of 27.03\% for Flower dataset but 62.5\% for Object dataset. SVM gave an accuracy of 33\% on Flower dataset while on object dataset it gave 84.375\% accuracy.

These results show that SVC classifier did great on Objects Dataset with an accuracy of 87\% and Random Forest got 62.5\% accuracy. But on Flowers dataset, it was giving an accuracy of less than 50\% with either of these classifiers and even K-Nearest Neighbours.


![Results](https://github.com/ZTHussain/Computer-Vision-A1/blob/2fb472558ef40cc3bdf40ca57d275942301ebafc/images/fig16.png)




