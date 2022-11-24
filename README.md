# TEAM_B
# Prediction of emojis from Twitter tweets using ML and DL models

![image](https://user-images.githubusercontent.com/90660841/190937288-6448f4de-d548-4f5e-8539-002db83834e0.png)


#### Dataset: [data](https://github.com/DATA-606-FALL-2022/TEAM_B/tree/main/Data)
#### Presentation: [Final presentation](https://github.com/DATA-606-FALL-2022/TEAM_B/blob/main/Final%20presentation.pptx)
#### Code: [notebooks](https://github.com/DATA-606-FALL-2022/TEAM_B/tree/main/Jupyter%20notebooks)
#### Youtube: [Youtube](https://www.youtube.com/watch?v=pHcBouGcb1I)

## 1. Project Overview
Text communications regularly include emojis, which are little, graphical representations of emotions or things, to enhance interpersonal communication. Here, the main objective is to develop a relationship between the text messages i.e tweets and the used emojis. The project is divided into phases, which include data collection, preprocessing, model construction, model training, and model evaluation. In order to predict emojis that make sense, our model aims to understand the underlying semantics of the text phrase using natural processing and deep learning techniques.

## 2. Data
The Twitter Emoji dataset consists of 50,000 tweets and their corresponding emoji labels. Therefore, there are 50,000 observations and 2 columns in this ("Tweet" and "Label"). Each tweet in the collection has a corresponding numerical label. Another text file has labels for different emojis, similar to the previous one. The emojis are among the top 20 most widely used emotions, and the labels range from 0 to 19. The labels with corresponding emojis are transformed from a txt file to a csv file using Python scripts.

![image](https://user-images.githubusercontent.com/112992802/202912661-b6f32a31-f9fd-4907-9ee1-728c5d6abe9d.png)

![image](https://user-images.githubusercontent.com/112992802/202912734-e124ca14-83f1-40c3-83aa-cae01779307b.png)

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
 
## 6. Count Vectorizer
Since machine learning algorithms cannot read raw text data, we must perform feature extraction on the text input in order to produce numerical feature vectors. In essence, count vectorization converts each word's frequency in a text to a number. The algorithms vectorize each text and count the number of times each unique word appears. Consequently, a document term matrix is produced that maintains track of the word counts for each word used in the vocabulary of each text document.

## 7. Machine Learning Models
With the help of count vectorizer we will be using machine learning models. We chose to utilize classification models because they work well with discrete features like word counts for text classification. Considering this, we have used the following models and we will do the model evaluation using classification report.

 * 7.1  Multinomial Naive Bayes
 * 7.2  Support Vector Machine
 * 7.3  LogisticRegression
 * 7.4  Decision Tree
 * 7.5  Random Forest
 * 7.6  XGBoost
 
 ## 8. Text Tokenization
Initially, the standard text preparation techniques are used to remove any noise from the data, such as hashtags, mentions, hyperlinks, punctuations etc.,
Now Each document is subjected to text tokenization, which enables vectorization of the entire text corpus by converting each text document into a series of integers. These numbers are the indices in a word dictionary that correspond to a specific token.
Example, 

Document - small throwback with my favorite guy

Sequence - [10, 72, 47, 11, 16, 45 ]

 * 8.1  Lastly, we will be performing the padding of sequences because each document consist of different length of sequence which is not suitable for deep learning approach.

![image](https://user-images.githubusercontent.com/112992802/202915345-1cb3b392-6ac7-4c15-8570-67f37c0ebe86.png)

### Difference b/w tokenization used in pre-processing and in deep learning
 
In pre-processing we have implemented tokenization as a process to remove stop words and to lemmatize the tweets. In deep learning we have approached for
'Text Tokenization' where it allows the document to form in a sequence(series of integers) whereas in pre-processing there is no formation of sequence     appearing for a set of tokens.

## 9. Deep learning models
With the help of text tokenization and padding of sequences we will be implementing the following deep learning models and we will do the model evaluation using classification report.

 * 9.1  Long short-term memory(LSTM)
 
 * 9.2  Bidirectional Long short-term memory(Bi-LSTM)
 
 * 9.3  Recurrent Neural Network(RNN)
 
## 10. Outcome of best model with high accuracy
 * 10.1 models accuracy comparision - Bi-Lstm has highest accuracy
 
 ![image](https://user-images.githubusercontent.com/112992802/202916197-33f6e243-4c00-4509-812e-6b0aa54a1c00.png)
 
 * 10.2 Comparision of avg accuracy of both the machine learning and deep learning models
 
 ![image](https://user-images.githubusercontent.com/112992802/202916331-7b3a0b3f-9229-4322-a6e0-9d38b6500463.png)
 
 * 10.3 Validation of emojis using best model i.e Bi-Lstm
 
 ![image](https://user-images.githubusercontent.com/112992802/202917131-f1e3af63-4340-4721-a301-1996bb30e427.png)
 
 ![image](https://user-images.githubusercontent.com/112992802/202917155-80fd7c65-a0e1-4d15-aee8-29f55d125e17.png)
 
## 11. Conclusion
 * 11.1  Machine learning algorithms have the drawback of attempting to divide each class along a line rather of identifying semantic relationships.
        Best Model - Bi-Directional LSTM (Deep learning approach)
        Accuracy – 91%

 * 11.2  In pre-processing we have implemented tokenization as a process to remove stop words and to lemmatize the tweets.
        In deep learning we have approached for ’Text Tokenization’ where it allows the document to form in a sequence(series of integers) whereas in             pre-processing there is no formation of sequence appearing for a set of tokens.
        
## References
Duminda, D. (2019, January 18). sentiment-analysis. https://medium.datadriveninvestor.com/sentiment-analysis-on-customer-tweets-nlp-c0eeaeffd19a

kim, R. (2018, January 10). twitter analysis. https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-4-count-vectorizer-b3f4944e51b5

GeeksforGeeks. (2022, July 7). Using CountVectorizer to Extracting Features from Text. https://www.geeksforgeeks.org/using-countvectorizer-to-extracting-features-from-text/

Mwiti, D. (2020, September 10). text classification. https://heartbeat.comet.ml/text-classification-using-long-short-term-memory-glove-embeddings-6894abb730e1
        
 


