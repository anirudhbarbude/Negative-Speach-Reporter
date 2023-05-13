# Negative-Speach-Reporter
ML classsification model to understand weather a speach or texts contain cuss words negative sentences

This code is a Python script that performs sentiment analysis on Twitter data using a decision tree classifier. The dataset used in this script is called "twitter.csv" and it contains tweets classified into three categories: "Hate Speech", "Offensive Language" and "No Hate and Offensive".

The script starts by importing necessary libraries including pandas, numpy, CountVectorizer, train_test_split, DecisionTreeClassifier, re, nltk, stemmer, stopwords, and string.

Then, the script reads the data from the "twitter.csv" file into a Pandas DataFrame and processes the data for analysis. The 'labels' column is created by mapping the 'class' column values using a dictionary to the actual sentiment labels. The script then selects only the 'tweet' and 'labels' columns and applies a cleaning function 'clean' to remove unwanted characters and punctuation marks from the tweets, convert all characters to lowercase, remove stop words, and stem the words to reduce the number of features.

After cleaning the tweets, the script converts the cleaned tweets into a numerical form using CountVectorizer() from the scikit-learn library. The data is then split into training and testing sets with a 33% ratio of testing data. The script then creates a DecisionTreeClassifier object and fits the model to the training data.

Finally, the script prompts the user to enter a text message, which is then transformed and predicted using the trained classifier model. The predicted sentiment label is printed as the output.

Overall, this code performs text classification of tweets using a decision tree classifier to predict the sentiment of the input text.
