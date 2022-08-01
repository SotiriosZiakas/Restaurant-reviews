# Restaurant-reviews

This is a Natural Language Processing project. 
The data is a tsv file consisting of two columns, the first contains the customers' reviews and the second whether they liked the restaurant or not in the form of 0s and 1s.

The idea is to first clean the text data following the steps:

1) Replace the punctuation with a space.
2) Make all the letters lowercase.
3) Remove the english stopwords.
4) Extract the root of every word so there are fewer different words and hence fewer columns later.

With the cleaned text data at hand, I now can use *CountVectorizer* to convert the text into vectors of 0s and 1s.

Next, I split the data into training and test sets using the *train_test_split* function and I use the *MultinomialNB* classifier which is suitable for classification with discrete features.

Lastly, I make predictions on the test set and evaluate the model using the *Confusion Matrix* and the *Accuracy Score* metrics.

As a quick test of the algorithm's performance, I make predictions for two new custom reviews.
