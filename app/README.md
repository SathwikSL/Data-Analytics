# 📱 Google Play Store Apps Analysis (EDA)

## 📖 Overview

This project performs **Exploratory Data Analysis (EDA)** on the **Google Play Store Apps** dataset and **User Reviews** dataset using Python. The project focuses on data cleaning, preprocessing, statistical analysis, and visualization to gain meaningful insights into app popularity, ratings, installs, and user sentiment.

---

## 📂 Repository Structure

```
app/
│
├── apps.ipynb
└── README.md
```

---

## 🎯 Project Objectives

- Clean and preprocess the datasets
- Analyze app categories
- Study app ratings and installs
- Compare free and paid apps
- Analyze user review sentiment
- Find relationships between important features
- Create informative visualizations

---

## 📊 Datasets

### apps.csv

Contains information about Google Play Store applications.

**Columns include:**
- App
- Category
- Rating
- Reviews
- Size
- Installs
- Type
- Price
- Genres
- Content Rating

---

### user_reviews.csv

Contains user review information.

**Columns include:**
- App
- Translated Review
- Sentiment
- Sentiment Polarity
- Sentiment Subjectivity

---

## 🧹 Data Cleaning

The following preprocessing steps are performed:

- Removed duplicate records
- Converted Rating into numeric values
- Filled missing Rating values using the median
- Converted Reviews into numeric values
- Cleaned Installs column by removing '+' and commas
- Converted Size into numeric format
- Replaced "Varies with device" with missing values
- Removed rows with missing Category values
- Removed reviews with missing Sentiment

---

## 📈 Exploratory Data Analysis

### 📌 Category Analysis

- Distribution of applications by category

### ⭐ Rating Analysis

- Rating distribution
- Free vs Paid app ratings
- Size vs Rating relationship

### 📥 Install Analysis

- Top 10 Most Installed Apps
- Ratings vs Installs

### 😊 Sentiment Analysis

- Sentiment distribution
- Sentiment polarity distribution

### 🔥 Correlation Analysis

Correlation between:

- Rating
- Reviews
- Installs

---

## 📊 Visualizations

The project generates:

- Count Plot
- Histogram
- Box Plot
- Scatter Plot
- Correlation Heatmap

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/google-play-store-eda.git
```

Move into the project folder:

```bash
cd google-play-store-eda
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## ▶️ Run the Project

```bash
python playstore_analysis.py
```

---

## 📚 Libraries Used

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

---

## 📌 Key Insights

- Most popular app categories
- Top installed applications
- Rating distribution across apps
- Comparison of free and paid apps
- Relationship between app size and ratings
- User review sentiment trends
- Correlation between ratings, reviews, and installs

---

## 🚀 Future Improvements

- Interactive Dashboard using Streamlit
- Power BI Dashboard
- Machine Learning Models
- NLP-based Sentiment Classification
- App Recommendation System
- Time Series Analysis

---

## 👨‍💻 Author

**Your Name**

GitHub: https://github.com/SatheikSL

---

## ⭐ Support

If you found this project useful, please ⭐ star this repository and share it with others!
