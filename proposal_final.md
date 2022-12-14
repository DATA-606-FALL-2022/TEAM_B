# TEAM_B

# DATA 606 PROJECT PROPOSAL

# Emoji Prediction from Twitter Data
## using Deep Learning and Machine Learning Approach
![image](https://user-images.githubusercontent.com/90660841/190937288-6448f4de-d548-4f5e-8539-002db83834e0.png)
![image](https://user-images.githubusercontent.com/90660841/190937294-8bec814a-226e-49c3-b7e1-1d9402c523fe.png)


## TEAM DESCRIPTION
This is a team project of Nese Tirki and Charishma Choudary Tummala.

## PROJECT OVERVIEW

* Emojis are tiny, pictorial representations of feelings or objects that are frequently used in text messages to improve interpersonal communication. Here, establishing a connection between the text messages and the emojis employed is the major goal. Data gathering, preprocessing, model development, model training, and model evaluation are the project's phases. The goal of the model we create is to comprehend the text sentence's underlying semantics utilizing natural processing and deep learning approaches to forecast emojis that make sense.


## Twitter and Emoji Data Sets 

https://www.kaggle.com/datasets/saivaibhav1/twitter-data-emoji?select=Twitter_Data.csv
https://www.kaggle.com/datasets/saivaibhav1/twitter-data-emoji?select=us_mapping.txt


## DATASET

The CodaLab Twitter Emoji dataset consists of 50,000 tweets and their corresponding emoji labels. So, here it consists of 50,000 observations and 2 columns("Tweet" and "Label").  There is a corresponding numerical label for each tweet in the collection. Similarly, there is one more txt data where each label corresponds to an individual emoji. The labels run from 0 to 19, and the emojis are among the 20 most popular emotions. Using Python scripts, the labels having corresponding emojis txt file is converted to a csv file.

# Processing tweets

* Natural language with which people communicate usually contain, commonly repeated words such as ‘a’, ‘an’ , ‘the’, which are commonly referred to as stop words. These words need to be filtered out before going for anymore further processing of the text since they do not greatly add any meaning of the sentence.
Next , lemmatization is applied on the text which determines the root word which belongs to the same language unlike stemming which only performs word reduction. Since lemmatization is typically more informative, it is opted over stemming. When lemmatization is applied to the words (‘eat’, ‘ate’, ‘eaten’) , it reduces the words to a common lemma which is ‘eat’.

** Removal of Stop words 

** Lemmatization of text

# Text Tokenization

* Implementation of text tokenization to help the document to form in a sequence i.e a series of integers which will be helpful for deep learning approach. The next step is followed by padding of sequences because each document will be having a different sequence length so in order to have a fixed sequence length we will be performing padding of sequences.


 ## UNIT OF ANALYSIS
 
 Label is the target variable. With the help of the "Tweet" feature, we are going to predict label emojis. For example, if the tweet is mentioned as "Love my work family Thank you" then the label assigned to it is 0 and the corresponding emoji for that label 0 is ❤️
 
## METHODOLOGY

* CountVectorization
* Multinomial Naïve Bayes Algorithm
* Support Vector Machines
* LogisticRegression
* DecisionTree
* Random Forest
* XGBoost
* Text Tokenization
* Long Short-Term Memory
* Bidirectional-LSTMs
* RRN
 
# Outcomes

* In this study, we present a couple of machine learning and deep learning models using tokenizations and will find out which model has high accuracy using classification report to predict the emoji symbol while comprehending the whole context of the statement and to develop the model in a simple and efficient manner.


## Team Roles and Responsibilities

### Nese

* Data collection.
* Exploratory Data Analysis
* Cleaning of the data.
* pre-processing data with tokenization
* Performing Machine learning modeling

### Charishma

* Performing CountVectorization.
* Performing Text Tokenization.
* Performing Deep learning modelling.
* Model comparison.
* Cross validating the results.
* Evaluating a best fit model for prediction.
