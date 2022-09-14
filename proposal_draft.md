# TEAM_B

# DATA 606 PROJECT PROPOSAL

# Skin Cancer classification prediction

## TEAM DESCRIPTION
This is a team project of Nese Tirki and Charishma Choudary Tummala.

## PROJECT OVERVIEW

* If there is a suspicion of skin cancer, the patient first undergoes a visual examination, and then clinical studies suitable for the disease begin.
* Early cancer diagnosis with Deep Learning (EI) techniques has recently been the most emphasized subject among researchers. In addition, as seen in many studies, medical
use in the field is gaining even more critical today.
* Researchers generally use DS techniques to diagnose cancer and cancer types in the health field.
* For example, due to the inaccuracy of Computed Tomography (CT) images in the diagnosis of lung cancer, experts have disagreements in making the right decision.
* In this article, we will analyze and examine the problem of classifying dermoscopic images of skin cancer, including lesions, using machine learning and deep learning techniques.

## BACKGROUND

* Sheha, Mariam A., et al. offer an automated approach for diagnosing melanoma using a series of dermoscopic pictures  (Sheha, 2012). To identify Melanocytic Nevi and Malignant Melanoma, features retrieved are based on gray level Co-occurrence matrix (GLCM) and Multilayer perceptron classifier (MLP). Automatic MLP and Traditional MLP were proposed as two separate training and testing strategies for the MLP classifier.

* Layode Oyebisi., et al., proposed an integrated decision support system for the automatic skin cancer recognition of pigmented skin lesions  (Layode, 2019). They used a deep learning model based on U-Net architecture that has been adapted for the segmentation of skin lesions which involves linking each pixel of an image to a class label. Then different features extracted from the pre-trained CNNs were fused together in all possible combinations using the Partial Least Square Canonical Correlation Analysis (CCA). 

## RESEARCH QUESTIONS:

1.  Is early cancer diagnosis possible with deep learning and machine learning?

2.  What is the content of the video and training in diagnosis?

3.  Appropriate methods can be used, in this case, what is their availability and how accurate is it?


## DATASET

For this analysis, we plan to get the dataset from https://data.mendeley.com/. The public dataset contains images and metadata about some patient details.

## UNIT OF ANALYSIS

* Our unit of analysis is to find out the type of skin cancer for patients. ~2298 samples of rows and 26 columns.

### What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?
 + We will be using 22 clinical features including the patient's age, skin lesion location, skin type, and skin lesion diameter.

### What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?
* We will be applying machine learning classification and deep learning CNN modelling.

## Below are the machine learning classification techniques:

* SGD Classifier
* OVO Classifier
* Random Forest Classifier
* Decision Tree Classifier
* Multinomial NB Classifier
* Multinomial Logistic Regression
 
 ## Below are the deep learning CNN technique:
 
* ResNet,
* MobileNet,
* GoogleNet,
* DenseNet


## How do you plan to develop/apply ML and how you evaluate/compare the performance of the models?

* Preprocess and analyze the metadata and construct various machine learning models to predict and evaluate the results of skin lesion classifications. Use image processing techniques and experiment with various prebuilt deep learning models on skin image data to evaluate the results of skin lesion classifications. Use prebuilt Convolutional Neural Networks (CNN) to inference missing values in columns of clinic tabular data. 
* Evaluate the performance of various models and find the best model for skin lesion classifications. Accuracy, f1 score and confusion matrix will be used to determine the performance of all the models. 

## What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?

* Skin cancer detection strategies based on machine learning and deep learning are comprehensively discussed and analyzed in this work. This project focuses on presenting skin cancer classification techniques using several machine learning and deep learning algorithms, which can be trained by both clinic tabular data and skin image data, outperforms other approaches.

## Team Roles and Responsibilities

### Charishma

* Data collection 
* Cleaning of the data.
* Exploratory Data Analysis.
* Performing Machine learning modeling.

### Nese

* Performing Deep learning CNN modelling
* Model comparison
* Cross validating the results
* Evaluating a best fit model for prediction.
