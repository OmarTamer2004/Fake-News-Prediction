Fake News Prediction using NLP & Logistic Regression

This project builds a machine learning model to detect fake news based on text content.
It uses Natural Language Processing (NLP) techniques and Logistic Regression for binary classification (Real vs Fake).

Technologies Used

Python

NumPy, Pandas

NLTK

Scikit-learn

TF-IDF Vectorizer

Logistic Regression

Matplotlib, Seaborn, WordCloud

Dataset

The dataset contains labeled news articles.

Loaded from:
/content/drive/MyDrive/train.csv

Columns
Column	Description
author	Name of the writer
title	Title of the news article
content	Combined (author + title)
label	0 = Real, 1 = Fake
NLP Preprocessing

The text is cleaned and normalized before training.

Remove non-alphabetic characters

Convert to lowercase

Remove stopwords (NLTK)

Apply Porter Stemming

Convert text to numerical features using TF-IDF

Model: Logistic Regression

Steps:

Split data (80% training, 20% testing)

Train Logistic Regression on TF-IDF vectors

Predict labels for training and test data

Evaluate performance

Evaluation Metrics

The script computes:

Training Accuracy

Test Accuracy

Precision

Recall

Confusion Matrix

R² Score

ROC Curve (AUC)

WordCloud for Fake and Real News

Example results (typical):

Train Accuracy: 98%
Test Accuracy: 93%
Precision: 0.94
Recall: 0.92

How to Run
1. Install dependencies
pip install numpy pandas scikit-learn nltk seaborn matplotlib wordcloud

2. Download stopwords
import nltk
nltk.download('stopwords')

3. Run the script
python fake_news_prediction.py

Visualizations Provided

Confusion Matrix

ROC Curve + AUC

WordCloud (Fake vs Real)

Accuracy comparison

Future Improvements

Use deep learning models (LSTM, GRU, BERT)

Include full article text instead of author + title

Hyperparameter tuning with GridSearchCV

Deploy using Flask or Streamlit

If you want, I can generate:

A shorter README

A more professional GitHub-style README

A version with badges (Python version, license, model accuracy)
