# 💳 Credit Card Fraud Detection with NLP and Machine Learning

## 📖 Overview

This project combines **Natural Language Processing (NLP)** and **Machine Learning** techniques to analyze a credit card transaction dataset for fraud detection. In addition to building predictive models, the project demonstrates text preprocessing, autocomplete, autocorrect, visualization, and algorithm comparison.

The project is implemented in **Python** using libraries such as **Pandas**, **NumPy**, **Scikit-learn**, **Matplotlib**, **Seaborn**, **TextBlob**, **NLTK**, and **WordCloud**.

---

# 📂 Repository Structure

```
Data-Analytics/
│
├── autocorrect/
    └── autocorrect.ipynb
    └── README.md
```

---

# 🎯 Project Objectives

- Load and explore the credit card transaction dataset
- Perform NLP preprocessing on transaction data
- Build an autocomplete system using N-Grams
- Implement autocorrect using TextBlob
- Train and evaluate Machine Learning models
- Compare different classification algorithms
- Visualize fraud detection insights
- Generate word clouds and confusion matrices

---

# 📊 Dataset Information

The dataset contains anonymized credit card transactions with the following features:

- Time
- Amount
- V1 to V28 (Anonymized Features)
- Class
  - **0** → Non-Fraud Transaction
  - **1** → Fraud Transaction

---

# 🧹 Data Preprocessing

The following preprocessing steps are performed:

- Loaded the dataset using Pandas
- Checked dataset shape and information
- Detected missing values
- Examined fraud class distribution
- Converted transaction records into text
- Cleaned text by:
  - Converting to lowercase
  - Removing special characters
  - Removing extra spaces

---

# 📝 Natural Language Processing (NLP)

## Text Generation

Each transaction is converted into a sentence such as:

```
Transaction amount 150.0 at time 100 class 0
```

### Text Cleaning

- Lowercase conversion
- Remove punctuation
- Remove unwanted characters
- Normalize whitespace

---

# 🔍 Autocomplete System

The project builds an autocomplete model using **Bi-Grams (N-Grams)**.

Example suggestions:

```
transaction →
amount →
time →
class →
```

---

# ✍️ Autocorrect

Misspelled words are corrected using **TextBlob**.

Example:

```
transction → transaction
amunt → amount
clas → class
tim → time
```

---

# 🤖 Machine Learning Models

The following algorithms are trained and evaluated:

- Logistic Regression
- Random Forest Classifier

---

# 📊 Performance Metrics

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score

---

# 📈 Visualizations

The project generates multiple visualizations including:

- Fraud vs Non-Fraud Distribution
- Transaction Amount Distribution
- Correlation Heatmap
- Word Cloud
- Confusion Matrix
- User Feedback Analysis
- Top 10 Frequent Words

---

# ⭐ User Experience Analysis

A sample user feedback dataset is created to visualize ratings.

Visualization:

- User Rating Distribution

---

# 🔄 Algorithm Comparison

The project compares:

| Algorithm | Metrics |
|-----------|----------|
| Logistic Regression | Accuracy, Precision, Recall, F1 Score |
| Random Forest | Accuracy, Precision, Recall, F1 Score |

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- TextBlob
- WordCloud
- Regular Expressions (re)

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/your-username/credit-card-fraud-nlp.git
```

Navigate to the project folder

```bash
cd credit-card-fraud-nlp
```

Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk textblob wordcloud
```

---

# ▶️ Run the Project

```bash
python fraud_detection.py
```

---

# 📚 Required Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import re

from collections import Counter

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import (
    accuracy_score,
    precision_score,
    recall_score,
    f1_score,
    confusion_matrix,
    ConfusionMatrixDisplay
)

from sklearn.feature_extraction.text import CountVectorizer

from nltk.util import ngrams
from textblob import TextBlob
from wordcloud import WordCloud
```

---

# 📌 Features

- ✔ Data Cleaning
- ✔ NLP Text Preprocessing
- ✔ Autocomplete System
- ✔ Autocorrect System
- ✔ Fraud Detection
- ✔ Logistic Regression
- ✔ Random Forest Classifier
- ✔ Performance Evaluation
- ✔ Algorithm Comparison
- ✔ Word Cloud Generation
- ✔ Correlation Analysis
- ✔ Confusion Matrix
- ✔ Data Visualization

---

# 🚀 Future Improvements

- Deep Learning Models (LSTM, GRU)
- Transformer-based NLP Models (BERT)
- Real-Time Fraud Detection
- Flask or Streamlit Web Application
- Interactive Dashboard using Power BI
- Hyperparameter Tuning
- Feature Engineering
- Model Deployment using Docker

---

# 📸 Sample Outputs

The project produces visualizations such as:

- Fraud Distribution Chart
- Transaction Amount Histogram
- Correlation Heatmap
- Word Cloud
- Confusion Matrix
- User Feedback Chart
- Top Frequent Words Bar Chart

---

# 👨‍💻 Author

**Your Name**

GitHub: https://github.com/SathwikSL

LinkedIn: https://www.linkedin.com/in/sathwik-s-l-657552386/

Email: slsathwik@gmail.com

---
