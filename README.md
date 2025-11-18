📰 Fake News Prediction using NLP & Logistic Regression

This project builds a machine learning model to detect fake news based on text content.
It uses Natural Language Processing (NLP) and Logistic Regression for binary classification (Real vs Fake).

🔧 Technologies Used

🐍 Python

📊 NumPy, Pandas

🧠 NLTK

🤖 Scikit-learn

📝 TF-IDF Vectorizer

📈 Logistic Regression

🎨 Matplotlib, Seaborn, WordCloud

📂 Dataset

The dataset contains labeled news articles.

Loaded from:
/content/drive/MyDrive/train.csv

📌 Columns
Column	Description
✍️ author	Name of the writer
📰 title	Title of the news article
📄 content	Combined (author + title)
🔖 label	0 = Real, 1 = Fake
🧹 NLP Preprocessing Steps

The text is cleaned and normalized before training.

🧼 Remove non-alphabetic characters

🔡 Convert to lowercase

🚫 Remove stopwords (NLTK)

✂️ Apply Porter Stemming

🔢 Convert text to TF-IDF numeric features

🤖 Machine Learning Model: Logistic Regression

Steps:

✂️ Train/Test split (80% / 20%)

🧠 Train Logistic Regression on TF-IDF vectors

🎯 Predict labels

📊 Evaluate performance

📈 Evaluation Metrics

The script computes:

✅ Training Accuracy

🧪 Test Accuracy

🎯 Precision

🔁 Recall

🧩 Confusion Matrix

📉 R² Score

📊 ROC Curve (AUC)

☁️ WordCloud (Fake vs Real)

Example results:

Train Accuracy: 98%
Test Accuracy: 93%
Precision: 0.94
Recall: 0.92

▶️ How to Run
1️⃣ Install dependencies
pip install numpy pandas scikit-learn nltk seaborn matplotlib wordcloud

2️⃣ Download stopwords
import nltk
nltk.download('stopwords')

3️⃣ Run the script
python fake_news_prediction.py

📊 Visualizations Included

🧩 Confusion Matrix

📈 ROC Curve + AUC

📊 Accuracy Comparison

☁️ Fake News WordCloud

☁️ Real News WordCloud

🚀 Future Improvements

🧠 Use deep learning models (LSTM / GRU / BERT)

📜 Use full article text instead of author + title

🎛️ Hyperparameter tuning (GridSearchCV)

🌐 Deploy using Flask or Streamlit
