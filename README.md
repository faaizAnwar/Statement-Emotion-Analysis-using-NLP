# Statement-Emotion-Analysis-using-NLP
In this Project, we'll develop a Sentiment Analysis model to categorize a statement as HAPPY, ANGRY or SAD

In the current phase of social media everyone are free to express their self. People's comment or reaction on a particular object justifies the opinion and the sentiments of the person. This feelings sometimes can be expressed in simple sentence order in a complex sentence.
Introducing a novel approach for classifying the the sentiments of the the comments what people make either on a object or to express themselves. This sentiments for the statement are classified as happy, sad or angry with respect to the query term.

This is very useful because it allows feedback to be aggregated without manual intervention. Here we use results of machine learning and natural language processing algorithms for classifying the sentiment. Our training data consists of comments with their TAG as happy , angry and sad.
Sentiment Analysis is the process of ‘computationally’ determining whether a piece of writing is positive, negative or neutral. It’s also known as opinion mining, deriving the opinion or attitude of a speaker.

PROPOSED SYSTEM:
The proposed system uses naive Bayes implementations: Bernoulli, multinational and Gaussian, and compared with their accuracy values. Later we impalement Neural Networks to find the emotion of the statement and accuracy for the emotion. The feature extraction procedure is implemented through browsing the data-set, cleaning and organizing, renaming the columns, deleting the unnecessary columns in the data-set. The trained data is obtained through splitting data-set into 2 splits train set and test set respectively.
The trained classifier models are used to classify the tweets in to positive and negative. The performance rate is measured through accuracy. Each of the algorithms is tested with their accuracy to determine the best model among all the other classifiers.

A. Import the libraries and data-set
The data set contains 635 statements stating Sad emotions, 708 statement stating happy emotions and 696 statements stating angry emotions.

B. Cleaning and visualizing the data-set
Text Preprocessing is traditionally an important step for Natural Language Processing (NLP) tasks. It transforms text into a more digestible form so that machine learning algorithms can perform better.
Lower Casing: Each text is converted to lowercase.
Replacing URLs: Links starting with "http" or "https" or "www" are replaced by "URL".
Replacing Emojis: Replace emojis by using a pre-defined dictionary containing emojis along with their meaning. (eg: ":)" to "EMOJIsmile")
Replacing Usernames: Replace @Usernames with word "USER". (eg: "@Kaggle" to "USER")
Removing Non-Alphabets: Replacing characters except Digits and Alphabets with a space.
Removing Stopwords: Stopwords are the English words which does not add much meaning to a sentence. They can safely be ignored without sacrificing the meaning of the sentence. (eg: "the", "he", "have")
Lemmatizing: Lemmatization is the process of converting a word to its base form. (e.g: “Great” to “Good”)

C. Splitting the dataset into train and test
The Preprocessed Data is divided into 2 sets of data:
Training Data: The dataset upon which the model would be trained on. Contains 70 % data.Test Data: The dataset upon which the model would be tested against. Contains 30% data.After splitting the shape of each set can be viewed. Each model will be trained based on the split data to understand the degree of accuracy. TF- IDF indicates what the importance of the word is in order to understand the document or dataset.
