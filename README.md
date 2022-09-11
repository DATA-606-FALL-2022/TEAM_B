# TEAM_B

# DATA 606 PROJECT PROPOSAL

# Skin Cancer classification prediction

## TEAM DESCRIPTION
This is a team project of Nese Tirki and Charishma Choudary Tummala.

## PROJECT OVERVIEW

Propaganda spreads the ideology and beliefs of like-minded people, brainwashing their audiences, and sometimes leading to violence.
Due to common reach of internet to the people, it has become easy for many sources to manipulate people to believe in something which is toxic and unhealthy by the use of the propaganda.
Propaganda news looks like the original news and it’s very difficult to identify as it is written very carefully. There are different ways through which we can identify it. Such as- • Having good knowledge over the topic • Focusing on words and topics where the stress is more.

## BACKGROUND

Though propaganda news classification is not a recent topic, but is an important one and in research for a long time. As the increase in social media use, there are many platforms and sources trying to populate their propaganda and feed to the people. The style of writing is also improving. So, there is a high scope of use of state-of-the-art model to identify the news and save many human minds to become toxic. There is a huge scope of improvement in this topic as there is very limited number of models and algorithms being implemented.

## RESEARCH QUESTIONS:

Why it is required to detect propaganda based news?

Which deep learning model can be used for efficient classification of propaganda based news?

How to create web application that can handle large dataset with proper data structure format?

Does contextual and linguistic features matter for such news classification?

## DATASET

The dataset comprises data extracted from https://zenodo.org/record/3271522#.Yxg-FuxN2SV .This project aims to build an efficient web based prototype for users which can classify the propaganda based news and articles from the actual ones.

## UNIT OF ANALYSIS

* Our unit of analysis is to find out the type of skin cancer for patients. ~2298 samples of observations are expected to be analyzed.

### What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?
 + We will using gender, age, skin_cancer, cancer_history

### What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?
* We will applying machine learning classification and deep learning CNN modelling.

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


## METHODOLOGY:

### How do you plan to develop/apply ML and how you evaluate/compare the performance of the models?

* Preprocess and analyze the metadata and construct various machine learning models to predict and evaluate the results of skin lesion classifications. Use image processing techniques and experiment with various prebuilt deep learning models on skin image data to evaluate the results of skin lesion classifications. Use prebuilt Convolutional Neural Networks (CNN) to inference missing values in columns of clinic tabular data. 
* Evaluate the performance of various models and find the best model for skin lesion classifications. Accuracy, f1 score and confusion matrix will be used to determine the performance of all the models. 

### What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?

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
