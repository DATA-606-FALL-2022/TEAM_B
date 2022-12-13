# TEAM_B
# Prediction of emojis from Twitter tweets using ML and DL models

![image](https://user-images.githubusercontent.com/90660841/190937288-6448f4de-d548-4f5e-8539-002db83834e0.png)


#### Link to Dataset: [data](https://github.com/DATA-606-FALL-2022/TEAM_B/tree/main/Data)
#### Link to Presentation: [Final presentation](https://github.com/DATA-606-FALL-2022/TEAM_B/blob/main/Final%20presentation.pptx)
#### Link to Code: [notebooks](https://github.com/DATA-606-FALL-2022/TEAM_B/tree/main/Jupyter%20notebooks)
#### Link to Youtube: [Youtube](https://www.youtube.com/watch?v=pHcBouGcb1I)

## Abstract
Text communications regularly include emojis, which are little, graphical representations of emotions or things, to enhance interpersonal communication. Here, the main objective is to develop a relationship between the text messages i.e tweets and the used emojis. The project is divided into phases, which include data collection, preprocessing, model construction, model training, and model evaluation. In order to predict emojis that make sense, our model aims to understand the underlying semantics of the text phrase using natural processing and deep learning techniques.

## 1. Introduction
Social media and cellphones have firmly established roots in how people text today. Emojis have sometimes taken the role of acronyms and abbreviations, but they are still crucial for social media and have a permanent impact on how we communicate. While some may find the use of emojis to be frivolous, there is no denying that they have improved the quality and nuance of our online communication. Since emoji have become commonplace worldwide, you can communicate with someone on the other side of the planet using the same icons. Emojis are one approach to improve internet communication as language changes with the times. The language of digital technology and communications is emojis, which are used more and more frequently online. Emoji are being utilized in online communications more frequently, and there are a growing number of different ways that they are being employed. Twitter has discovered that several popular emoticons have replaced many early online slang terms because they have meanings that are similar to those phrases. The intended meanings of the emoji have also evolved over time to become more caustic or sardonic, even with the aim of conveying your emotional condition to the recipient of your message.

## 2. Data
The Twitter Emoji dataset consists of 50,000 tweets and their corresponding emoji labels. Therefore, there are 50,000 observations and 2 columns in this ("Tweet" and "Label"). Each tweet in the collection has a corresponding numerical label. Another text file has labels for different emojis, similar to the previous one. The emojis are among the top 20 most widely used emotions, and the labels range from 0 to 19. The labels with corresponding emojis are transformed from a txt file to a csv file using Python scripts.

![image](https://user-images.githubusercontent.com/112992802/202912661-b6f32a31-f9fd-4907-9ee1-728c5d6abe9d.png)

![image](https://user-images.githubusercontent.com/112992802/207419062-9090bbb3-3c62-478d-88be-17275b37c617.png) ![image](https://user-images.githubusercontent.com/112992802/207419140-5ca715f8-d34e-4e70-b463-ee29f0502b15.png)

## 3. Data Cleaning
Numbers, punctuation, linked texts, and other user mentions (@) are frequently used in tweet texts. We will be deleting all the unnecessary data so that the data may be understood if presented in a clear format.

 * 3.1  Initially, for convenience, all capital letters have been removed from the text.
 
 * 3.2  All retweet tags(RT), user mentions (@user), and hashtag symbols (#) has been removed.
 
 * 3.3  All hyperlinks has been removed
 
 * 3.4  All tweets containing numbers has been removed

 * 3.5  All punctuations in the tweets has been removed
 
## 4. Data Pre-processing
The conversion of the raw material into a comprehensible format is known as data pre-processing. Data preprocessing is a crucial step for a data before its actual use to increase data effectiveness. Before applying the algorithm, the dataset is preprocessed to look for missing values, noisy data, and other inconsistencies.
 
 * 4.1  Spacy is used as part of tokenization in order to perform removal of stop words and lemmatization of tweet.
 
 * 4.2  Stop words, also known as commonly used words like "a," "an," and "the," are frequently seen in people's everyday conversations. These words should be eliminated before carrying out any further text processing because they rarely add to the meaning of the text's expression.
 
 * 4.3  Following that, the text is subjected to lemmatization, which, in contrast to stemming, which only reduces words, identifies the root word that is native to the same language. Lemmatization is favored to stemming because it is frequently more illuminating. Only the word "eat" survives as the common lemma after lemmatizing the terms "eat," "ate," and "eaten."
 
## 5. Visualizations
 * 5.1 Label count distribution
 
 ![image](https://user-images.githubusercontent.com/112992802/202914542-37afbf7b-696b-47d4-bba4-fa85739d95c0.png)
 
 * 5.2 Length of tweets distribution
 
 ![image](https://user-images.githubusercontent.com/112992802/202914617-7935f6c8-a853-4fa9-a550-4e3ce3179236.png)
 
 ## 6. Unit of Analysis
Label is the target variable. With the help of the "Tweet" feature, we are going to predict label emojis. For example, if the tweet is mentioned as "Love my work family Thank you" then the label assigned to it is 0 and the corresponding emoji for that label 0 is ❤️. In this study, we present a couple of machine learning and deep learning models using countvectorizer and text-tokenization and will find out which model has high accuracy using classification report to predict the emoji symbol while comprehending the whole context of the statement and to develop the model in a simple and efficient manner.
 
## 7. Count Vectorizer
Since machine learning algorithms cannot read raw text data, we must perform feature extraction on the text input in order to produce numerical feature vectors. In essence, count vectorization converts each word's frequency in a text to a number. The algorithms vectorize each text and count the number of times each unique word appears. Consequently, a document term matrix is produced that maintains track of the word counts for each word used in the vocabulary of each text document.
![image](https://user-images.githubusercontent.com/112992802/207406449-d69675c1-5f3b-42d3-b204-8ae0cf9e3b2c.png)

## 8. Machine Learning Models
With the help of count vectorizer we will be using machine learning models. We chose to utilize classification models because they work well with discrete features like word counts for text classification. Considering this, we have used the following models and we will do the model evaluation using classification report.

 * 8.1  Multinomial Naive Bayes
 * 8.2  Support Vector Machine
 * 8.3  LogisticRegression
 * 8.4  Decision Tree
 * 8.5  Random Forest
 * 8.6  XGBoost
 
 ![image](https://user-images.githubusercontent.com/112992802/207413517-e6444c6d-5632-4410-857b-a6ffc9824748.png) ![image](https://user-images.githubusercontent.com/112992802/207413769-1ad8a0c0-ecbc-4835-b0ef-d78cbf367d8c.png)
 
 ![image](https://user-images.githubusercontent.com/112992802/207412232-8a55c106-5b2e-4ae4-8bf5-a117bec878ed.png)  ![image](https://user-images.githubusercontent.com/112992802/207412466-72c924e0-93a2-49da-b7dd-2a0653f6a90a.png)
 
 ![image](https://user-images.githubusercontent.com/112992802/207412855-d0e8c01d-ea1f-4a5b-aef2-2ab2b5d51ed2.png)  ![image](https://user-images.githubusercontent.com/112992802/207413227-60938836-bb05-40cb-8f0a-adbd07027967.png)

 
## 9. Text Tokenization
Initially, the standard text preparation techniques are used to remove any noise from the data, such as hashtags, mentions, hyperlinks, punctuations etc.,
Now Each document is subjected to text tokenization, which enables vectorization of the entire text corpus by converting each text document into a series of integers. These numbers are the indices in a word dictionary that correspond to a specific token.
Example, 

Document - small throwback with my favorite guy

Sequence - [10, 72, 47, 11, 16, 45 ]

 * 9.1  Lastly, we will be performing the padding of sequences because each document consist of different length of sequence which is not suitable for deep learning approach.

![image](https://user-images.githubusercontent.com/112992802/202915345-1cb3b392-6ac7-4c15-8570-67f37c0ebe86.png)

### Difference b/w tokenization used in pre-processing and in deep learning
 
In pre-processing we have implemented tokenization as a process to remove stop words and to lemmatize the tweets. In deep learning we have approached for
'Text Tokenization' where it allows the document to form in a sequence(series of integers) whereas in pre-processing there is no formation of sequence     appearing for a set of tokens.

## 10. Deep learning models
With the help of text tokenization and padding of sequences we will be implementing the following deep learning models and we will do the model evaluation using classification report.

 * 10.1  Long short-term memory(LSTM)
 * 10.2  Bidirectional Long short-term memory(Bi-LSTM)
 * 10.3  Recurrent Neural Network(RNN)
 
 ![image](https://user-images.githubusercontent.com/112992802/207414218-3e26e106-e664-487f-a98e-6eaf08125a4d.png)  ![image](https://user-images.githubusercontent.com/112992802/207414463-336b4526-963a-40ba-9913-c7014944ccd6.png)
 
 ![image](https://user-images.githubusercontent.com/112992802/207414710-0cbc6b1e-8399-4d57-aa01-c35360d458a8.png)

## 11. Outcome of best model with high accuracy
 * 11.1 models accuracy comparision - Bi-Lstm has highest accuracy
 
 ![image](https://user-images.githubusercontent.com/112992802/207414991-c4ae3b02-8a27-48c3-997b-cb11255f27b1.png)
 
 * 11.2 Comparision of avg accuracy of both the machine learning and deep learning models
 
 ![image](https://user-images.githubusercontent.com/112992802/207415252-ba555de2-45e3-411f-89c8-11626572eb6a.png)
 
 * 11.3 Validation of emojis using best model i.e Bi-Lstm
 
 ![image](https://user-images.githubusercontent.com/112992802/202917131-f1e3af63-4340-4721-a301-1996bb30e427.png)
 
 ![image](https://user-images.githubusercontent.com/112992802/202917155-80fd7c65-a0e1-4d15-aee8-29f55d125e17.png)
 
## 12. Conclusion and Future Work
 * 12.1   Machine learning algorithms have the drawback of attempting to divide each class along a line rather of identifying semantic relationships.
   Best Model - Bi-Directional LSTM (Deep learning approach)
   Accuracy – 91%

 * 12.2   In pre-processing we have implemented tokenization as a process to remove stop words and to lemmatize the tweets.
   In deep learning we have approached for ’Text Tokenization’ where it allows the document to form in a sequence(series of integers) whereas in              pre-processing there is no formation of sequence appearing for a set of tokens.
        
 * 12.3   Deep learning approaches especially LSTM's have high chances of understanding the semantic relationships between the texts. Emojis fill a      communication gap in texting. When compared to the social signs we pick up through spoken communication, this is the best. Emojis and emoticons can lessen the possibility of information ambiguity in a similar way as body language does in face-to-face interactions. In future, we will be implementing more numbers of emojis with their corresponding labels. So that the communication via texts will have much more efficiency.
        
## References
Duminda, D. (2019, January 18). sentiment-analysis. https://medium.datadriveninvestor.com/sentiment-analysis-on-customer-tweets-nlp-c0eeaeffd19a

kim, R. (2018, January 10). twitter analysis. https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-4-count-vectorizer-b3f4944e51b5

GeeksforGeeks. (2022, July 7). Using CountVectorizer to Extracting Features from Text. https://www.geeksforgeeks.org/using-countvectorizer-to-extracting-features-from-text/

Mwiti, D. (2020, September 10). text classification. https://heartbeat.comet.ml/text-classification-using-long-short-term-memory-glove-embeddings-6894abb730e1
        
 


