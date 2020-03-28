# Histopathologic Cancer Detection

The aim of this project is to identify metastatic cancer in small image patches taken from larger digital pathology scans and to classify them as either cancerous or not cancerous.

Please note this project is a work in progress.

### Table of Contents
* [Technologies Used](https://github.com/sarina-amin/histopathologic-cancer-detection/blob/master/README.md#technologies-used)
* [Packages Used](https://github.com/sarina-amin/histopathologic-cancer-detection/blob/master/README.md#packages-used)
* [Methods Used](https://github.com/sarina-amin/histopathologic-cancer-detection/blob/master/README.md#methods-used)
* [The Project](https://github.com/sarina-amin/histopathologic-cancer-detection/blob/master/README.md#the-project)
    * [Gathering Data](https://github.com/sarina-amin/histopathologic-cancer-detection/blob/master/README.md#gathering-data)
    * [Exploratory Data Analysis]
    * [Modelling]
* [Final Thoughts and Areas for Further Exploration]

### Technologies Used
* Python
* Jupyter Notebook

### Packages Used
* **glob** - easily finding matching filenames
* **numpy** - because it is the math module for most things
* **pandas** - a powerful module for data structures and - analysis
* **keras** - a high-level deep learning API, in this case to ease TensorFlow usage
* **cv2** - for image processing (we'll just use it for loading images)
* **tqdm** - a minimalistic yet powerful and easy to use progress bar
* **matplotlib** - a plotting module
* **gc** - garbage collection to save RAM

### Methods Used 
* Convolutional Neural Networks
* Data Visualisation

## The Project

### Gathering Data

The dataset I used was from a Kaggle competition called Histopathologic Cancer Detection, the full challenge and data set can be found here: https://www.kaggle.com/c/histopathologic-cancer-detection/overview

It contained microscopic images of lymph node tissue with a resolution of 96x96 pixels. The dataset contains a total of 220,025 training images and 57,458 testing images. Each image has been labelled as 0 (negative for cancer tissue) or 1 (positive for cancer tissue). A positive label indicates that the centre 32x32 pixels region of a patch contains at least one pixel of tumor tissue. Tumor tissue in the outer region of the patch does not influence the label.
Data cleaning was not required.


### Exploratory Data Analysis

