# 🐦 Twitter Sentiment Analysis using Machine Learning

A Natural Language Processing (NLP) project that classifies tweets as **Positive** or **Negative** using Machine Learning. The project performs text preprocessing, feature extraction with TF-IDF, and sentiment classification using Logistic Regression.

---

## 📌 Project Overview

Twitter is one of the largest platforms where people express their opinions about products, events, brands, and social issues. This project uses Natural Language Processing (NLP) techniques to analyze tweets and determine whether their sentiment is positive or negative.

The project was implemented in **Google Colab**, and the dataset was downloaded directly from **Kaggle** using the **Kaggle API**.

---

## 📂 Dataset

**Dataset:** Sentiment140

- Source: Kaggle
- Total Tweets: 1.6 Million
- Labels:
  - 0 → Negative
  - 4 → Positive

Dataset contains:

- Target
- Tweet ID
- Date
- Query
- Username
- Tweet Text

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Kaggle API
- Pandas
- NumPy
- NLTK
- Regex (re)
- Scikit-learn
- Pickle

---

## 📚 Python Libraries

```python
import numpy as np
import pandas as pd
import re
import nltk
from nltk.corpus import stopwords
from nltk.stem.porter import PorterStemmer
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
import pickle
```

---

## 🔄 Project Workflow

1. Import required libraries
2. Download dataset using Kaggle API
3. Load dataset into Pandas
4. Data preprocessing
5. Remove special characters
6. Convert text to lowercase
7. Remove stopwords
8. Apply Porter Stemming
9. Convert text into TF-IDF vectors
10. Split data into training and testing sets
11. Train Logistic Regression model
12. Evaluate model accuracy
13. Save trained model using Pickle
14. Predict sentiment of new tweets

---

## 🧹 Text Preprocessing

The following preprocessing steps were applied:

- Lowercase conversion
- Removal of URLs
- Removal of usernames
- Removal of punctuation
- Removal of numbers
- Stopword removal
- Porter Stemming

---

## 🤖 Machine Learning Model

**Algorithm Used**

- Logistic Regression

**Feature Extraction**

- TF-IDF Vectorization

---

## 📊 Model Evaluation

Evaluation Metrics:

- Training Accuracy
- Testing Accuracy
- Accuracy Score

---

## 📁 Project Structure

```
Twitter-Sentiment-Analysis/
│
├── Twitter_Sentiment_Analysis.ipynb
├── README.md
├── requirements.txt
├── trained_model.sav
└── kaggle.json
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/sharwahodgar/Twitter_Sentiment_Analysis
```

### Install Dependencies

```bash
pip install numpy pandas nltk scikit-learn kaggle
```

---

## Kaggle API Setup

Upload your `kaggle.json` file in Google Colab.

```python
from google.colab import files
files.upload()

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

Download the dataset:

```bash
!kaggle datasets download -d kazanova/sentiment140
```

Extract the dataset:

```bash
!unzip sentiment140.zip
```

Run all notebook cells to train the model and perform sentiment prediction.

---

## 🎯 Features

- Twitter sentiment classification
- NLP preprocessing pipeline
- TF-IDF feature extraction
- Logistic Regression classifier
- Model serialization using Pickle
- Prediction on custom tweet text

---

## 📖 Learning Outcomes

- Natural Language Processing (NLP)
- Text Cleaning
- Feature Engineering
- TF-IDF Vectorization
- Machine Learning Classification
- Logistic Regression
- Model Evaluation
- Model Serialization
- Working with Kaggle API
- Google Colab Workflow

---

## 👩‍💻 Author

**Sharwa Hodgar**

- GitHub: https://github.com/sharwahodgar
- LinkedIn: https://www.linkedin.com/in/sharwahodgar/

---
