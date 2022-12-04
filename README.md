# Consumer-complaints-classification
The objective is to develop supervised machine learning frameworks to classify each complaint of the given corpus into one of five categories: credit reporting, debt collection, mortgages and loans, credit cards and retail banking using text feature extraction and text classification techniques


## Methods
In the beginning of the project, visualization of distribution of the complaints data into each category was done. The training data consists of 158350 complaints and the test data consists of 4060 complaints. 
We observed that the data is skewed towards credit reporting with almost half of the text in this category.
Ten null complaints were removed since they did not give any information about their categorization.
Text cleaning was done to remove the punctuation marks and make the data case-insensitive. Pre-processing of text involved Tokenization, 
Stemming, Lemmatization, and stop-words removal.

The feature extraction was done using tf-idf, bag of words, and bag of words with ngrams
of range (1,2), (2,3) and (1,3). They were used to transform the words into vectors for further
processing of corpus of complaints.
To evaluate the performance of classifiers, 80% of complaints are used for training purpose and rest
20% complaints are used for cross validation with stratified class labels. A pipeline has been created
using 5 models that are Logistic Regression, Decision Tree, Random Forest, Multinomial Na ̈ıve Bayes
and k-Nearest Neighbor Classifier along with Grid Search parameter tuning technique. These models
have been implemented using the scikit-learn library of Python.


