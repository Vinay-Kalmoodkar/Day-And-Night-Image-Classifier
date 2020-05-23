# Day-And-Night-Image-Classifier

## Problem Statement
It is a **COMPUTER VISION** task. The main idea is to build a classifier that predicts whether a given image is a Day image or Night image **WITHOUT USING NEURAL NETWORKS.**

## About Dataset
The 200 day/night images are separated into training and testing datasets. 
* 60% of these images are training images, for you to use as you create a classifier.
* 40% are test images, which will be used to test the accuracy of your classifier.

## Feature Extraction
Create a feature that represents the brightness in an image. We'll be extracting the **average brightness using HSV colorspace.** Specifically, we'll use the **V channel (a measure of brightness)**, add up the pixel values in the V channel, then divide that sum by the area of the image to get the average Value of the image.

## Classification
We set a threshold for brightness say `thresh`. We compare the brightness of each image say  `image[i]` with this threshold `thresh`, if   `image[i]` **>** `thresh` we assign it as **Day image** or else **Night image**

## Evaluation and Visualization
We use **accuracy** metric for evaluation as we have balanced dataset. **Matplotlib** is used for visualizing the images that are incorrectly classified.
