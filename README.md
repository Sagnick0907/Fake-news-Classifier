# Fake-News-Classifier

## Table of Content
  * [Overview](#overview)
  * [Technical Aspect](#technical-aspect)
  * [Technologies Used](#technologies-used)

## Overview
This is a Fake News Classifier using - CountVectorizer(Bag Of Words), TfID Vectorizer, Hashing Vectorizer trained on MultinomialNB Algorithm, Passive Aggressive Classifier Algorithm, MultinomialNB Algorithm with Hyper Parameter Tuning.  

## Technical Aspect
Dataset Link: https://www.kaggle.com/c/fake-news/data?select=submit.csv  
Given below are the steps taken to build the model:  
For the NLP implementation code –  
  - Imported necessary **Python libraries** (Pandas, re, nltk, sklearn, etc.)
  -	Imported the Dataset, dropped rows containing missing data, reset the index.
  -	In **Data cleaning** & **Text pre-processing** Section, we removed all unnecessary symbols & numbers. We lower cased all sentences & split sentences into words.
  -	Performed **removal of stopwords** and **Stemming**.
  -	Used **CountVectorizer(Bag Of Words), TfID Vectorizer, Hashing Vectorizer** in their respective code file.
  -	Performed a **train_test_split** on labels & messages.
  -	Trained & tested the model using **MultinomialNB Classifier**, **Passive Aggressive Classifier** & **MultinomialNB Classifier with Hyper Parameter Tuning**.
  -	From sklearn we imported **metrics** to produce Accuracy & confusion_matrix for our model.  
| Vectorizer | ML model | Accuracy |
| --- | --- |
| CountVectorizer | MultinomialNB Algorithm | 0.902 |
| CountVectorizer | Passive Aggressive Classifier | 0.918 |
| CountVectorizer | MultinomialNB Classifier(Hyper Parameter Tuning) | 0.9026 |
| TfID Vectorizer | MultinomialNB Algorithm | 0.900 |
| TfID Vectorizer | MultinomialNB Classifier(Hyper Parameter Tuning) | 0.9022 |
| HashingVectorizer | MultinomialNB Algorithm  | 0.876 |
      
## Technologies Used
- Jupyter Notebook
-	ML model: MultinomialNB Algorithm, Passive Aggressive Classifier, MultinomialNB Classifier with Hyper Parameter Tuning (Selected)
-	Libraries: pandas, re, nltk, sk-learn.
