			This project case study was done as a part of course by appliedaicourse.com . The problem statment is from a kaggle competion where we were needed to find similarity between two quora questions so that portal can mark a question duplicate of other.

Steps followed for approaching the solution:

1. Data Collection : Data was taken and is available at kaggle (https://www.kaggle.com/c/quora-question-pairs/data)

2. EDA was done to analyse and extract insights of data present.

3. Data Pre-processing : Various pre-processing meausures were implemented like Removing html-tags/Punctuations/Stopwords, performing stemming etc.

4. NLP advance feature Engineering : Some advance NLP features were extracted from the data and wordcloud was also plotted for both duplicated as well as non-duplicate questions to see most frequently used words in both the sets.

5. Feature Engineering : All the text data was vectorized using tfidf/tfidf-weighted-word2vec and scaling was done on numerical features then all the features of both the questions were concatinated for feeding it to ML models

6. ML models : As we were using log-loss as peformance matric , we needed to calculate worst case log loss i.e. for random model to set our baic benchmark for the Model performance. Logistic regression,Linear SVM and xgboost algorithms were applied on the dataset with hyperparameter tuning to find log-loss and at the end summarized all the results.

Referance :

• Source : 
https://www.kaggle.com/c/quora-question-pairs

• Discussions :
https://www.kaggle.com/anokas/data-analysis-xgboost-starter-0-35460-lb/comments

• Kaggle Winning Solution and other approaches:
https://www.dropbox.com/sh/93968nfnrzh8bp5/AACZd

• Blog 1 : 
https://engineering.quora.com/Semantic-Question-Matching-with-Deep-Learning

• Blog 2 : 
https://towardsdatascience.com/identifying-duplicate-questions-on-quora-top-12-on-kaggle-4c1cf93f1c30
