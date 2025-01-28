<h2 align="center"> Machine Learning algorithm for Sentiment Analysis of IMDB </h1>

### 📌 Project description

- This project have objective the construction of machine learning model with >80% accuracy capabe of classify whether a user review has positive or negative connotation.

### 📜 Dataset

- Dataset used was IMDB (Internet Movie Database) of 50k Movie review from Kaggle. It comprise of two collumns: one with user's review and one with review's sentiment classified as "positive" or "negative".
- Link: https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

### 📚 Libraries

Python libraries used for this project are:

- re
- pickle
- nltk
- sklearn
- numpy
- pandas
- nltk
- sklearn

### 🗑️ Data Cleaning

First of all, data cleaning step was applied to convert sentiment column into numeric binary classifiation ("1" = "positive" and  "0" = "negative") and remove HTML tags and special characters from reviews.
In additional, Natural Language Processing (NLP) techniques were used to remove stopwords and apply stemming into users reviews to standardize the words for the data pre-processing step. 

### 📍 Data pre-processing

In this step, dataset was divede into 80% trainning and 20% test. Also, data was converted into numerical representation, creating a vector using sklearn library and after transform into array NumPy.

### ⚙️ Data model machine learning

To test accuracy >80%, three distributions supervised machine learning of classification were created based on Naive Bayes algorithm: 
- GaussianNB
- MultinomialNB
- BernoulliNB

### 📊 Results

To check accuracy of each model, was used AUC (Area Under The Curve), a metric for evaluating the performance of classification models in machine learning.
So, here we are:

- AUC GaussianNB = 0.6668474355243407
- AUC MultinomialNB = 0.8071783917411954
- AUC BernoulliNB = 0.8188667244694989

BernoulliNB presented best performanced in relation to others models.

