
# 🍷 Wine Quality Prediction 

## 📖 Overview

This project focuses on **Wine Quality Prediction** using machine learning techniques. The workflow includes data analysis, exploratory data analysis (EDA), data preprocessing, feature scaling, model training, and performance comparison of multiple classification algorithms.

The objective is to predict the quality of wine based on its physicochemical properties and identify the features that have the greatest impact on wine quality.

---

# 📂 Repository Structure

```text
wine/
│
├── WineQT.csv
├── wine.ipynb
└── README.md
```

---

# 📊 Dataset Information

The dataset contains physicochemical properties of wine samples along with their quality ratings.

### Features

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality (Target Variable)

> **Note:** The `Id` column is removed before model training as it does not contribute to prediction.

---

# 🎯 Project Objectives

- Explore the wine quality dataset
- Analyze feature distributions and relationships
- Visualize important patterns in the data
- Preprocess data for machine learning
- Train multiple classification models
- Compare model performance
- Identify the most influential features affecting wine quality

---

# 🧹 Data Analysis

The project begins with a detailed analysis of the dataset, including:

- Displaying the first five records
- Dataset dimensions
- Data types
- Summary statistics
- Missing value analysis
- Quality class distribution
- Correlation analysis

---

# 📊 Exploratory Data Analysis (EDA)

Several visualizations are created to better understand the dataset.

### Wine Quality Distribution

- Count Plot showing the frequency of each quality rating.

### Correlation Heatmap

- Displays correlations between all numerical features.

### Alcohol vs Wine Quality

- Box Plot showing how alcohol content varies across different quality levels.

### Density vs Wine Quality

- Scatter Plot illustrating the relationship between density and wine quality.

---

# ⚙️ Data Preprocessing

The following preprocessing steps are performed:

### Remove Unnecessary Features

- Dropped the `Id` column.

### Feature and Target Separation

- **Features (X):** All physicochemical properties
- **Target (y):** Wine Quality

### Train-Test Split

- Training Data: **80%**
- Testing Data: **20%**
- Random State: **42**
- Stratified sampling to maintain class balance

### Feature Scaling

Numerical features are standardized using **StandardScaler** for algorithms that require normalized input.

---

# 🤖 Machine Learning Models

Three classification algorithms are implemented and compared.

## 1️⃣ Random Forest Classifier

An ensemble learning algorithm that builds multiple decision trees and combines their predictions.

**Accuracy:** **71.6%**

---

## 2️⃣ Support Vector Classifier (SVC)

A supervised learning algorithm that classifies data by finding the optimal decision boundary.

**Accuracy:** **66.8%**

---

## 3️⃣ Stochastic Gradient Descent (SGD) Classifier

A linear classifier optimized using stochastic gradient descent.

**Accuracy:** **57.6%**

---

# 📊 Model Comparison

The accuracy of all models is compared using a bar chart.

| Model | Accuracy |
|--------|----------|
| Random Forest | 71.6% |
| Support Vector Classifier | 66.8% |
| SGD Classifier | 57.6% |

---

# 🌟 Feature Importance

Feature importance scores are extracted from the **Random Forest Classifier** to determine which physicochemical properties contribute the most to predicting wine quality.

The results are displayed in descending order of importance.

---

# 📈 Visualizations

The notebook generates the following visualizations:

- Wine Quality Distribution
- Correlation Heatmap
- Alcohol vs Quality Box Plot
- Density vs Quality Scatter Plot
- Model Comparison Bar Chart

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📚 Python Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler

from sklearn.ensemble import RandomForestClassifier
from sklearn.linear_model import SGDClassifier
from sklearn.svm import SVC

from sklearn.metrics import accuracy_score
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/SathwikSL/Data-Analytics.git
```

Navigate to the project directory:

```bash
cd Data-Analytics/wine
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

# ▶️ Running the Project

Launch the Jupyter Notebook:

```bash
jupyter notebook wine.ipynb
```

---

# 📌 Features

- ✔ Data Analysis using Pandas
- ✔ Exploratory Data Analysis (EDA)
- ✔ Missing Value Analysis
- ✔ Correlation Analysis
- ✔ Feature Scaling
- ✔ Train-Test Split
- ✔ Random Forest Classification
- ✔ Support Vector Classification
- ✔ SGD Classification
- ✔ Model Performance Comparison
- ✔ Feature Importance Analysis
- ✔ Data Visualization

---

# 📂 Project Outputs

The notebook generates:

- Dataset Summary
- Missing Value Report
- Quality Distribution Chart
- Correlation Heatmap
- Alcohol vs Quality Box Plot
- Density vs Quality Scatter Plot
- Model Accuracy Comparison
- Feature Importance Ranking

---

# 📊 Performance Summary

| Model | Accuracy |
|--------|----------|
| 🌲 Random Forest | **71.6%** |
| 🎯 Support Vector Classifier | **66.8%** |
| ⚡ SGD Classifier | **57.6%** |

**Best Performing Model:** Random Forest Classifier

---

# 🚀 Future Enhancements

- Hyperparameter Tuning with GridSearchCV
- XGBoost Classifier
- LightGBM Classifier
- CatBoost Classifier
- Cross-Validation
- ROC Curve & AUC Analysis
- Confusion Matrix Visualization
- Streamlit Web Application
- Wine Quality Prediction API

---

# 🎯 Learning Outcomes

This project demonstrates how to:

- Explore and analyze structured datasets
- Perform exploratory data analysis (EDA)
- Visualize feature relationships
- Prepare data for machine learning
- Train and compare multiple classification models
- Evaluate model performance
- Interpret feature importance in ensemble models

---

# 👨‍💻 Author

**Sathwik S L**

GitHub: https://github.com/SathwikSL

---


If you found this project useful, please consider giving the repository a **⭐ Star** and feel free to contribute through issues or pull requests.

