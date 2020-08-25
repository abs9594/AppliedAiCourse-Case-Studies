    This project case study was done as a part of course by appliedaicourse.com. The problem statment is taken from a kaggle competion where we were needed to find relavent tags for questions posted on stackoverflow.

Steps followed for approaching the solution:

1. Data Collection : Data was taken and is available at kaggle (https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data)

2. EDA was done to analyse and extract insights of data like number of question,average number of tags, duplicate questions etc and appropriate performance metric i.e. micro F1 Score was selected

3. Data Pre-processing : Various pre-processing meausures were implemented like duplicate rows removal,Removing html-tags/Punctuations/Stopwords, performing stemming etc on the text features i.e title and description

4. Sampling of questions and number of tags were done so that we can run it on less computationaly powered machines as well

5. Feature Engineering : We observed that in any question, the most important things is always written in summary so we increaed weightage of summary 3 times in the text feature then the text data was vectorized using tfidf/BOW vectorizer

6. ML models : As we had this problem of multi-label classification, we used oneVsrest classifier as it works both for multiclass as well multilabel problems.We tried SGDClassifier with log loss as well as Logistic Regression classifier as base model in oneVsrest using different ngrams range and at the end summarized all the results.

Referance :
 
• Data Source : 
	https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data

• Youtube :
	https://youtu.be/nNDqbUhtIRg

• Research papers:
	https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tagging-1.pdf
	https://dl.acm.org/citation.cfm?id=2660970&dl=ACM&coll=DL
