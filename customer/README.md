
# 🛍️ Customer Personality Analysis & Segmentation using Machine Learning

## 📖 Overview

This project focuses on **Customer Personality Analysis** using data preprocessing, exploratory data analysis (EDA), feature engineering, and **K-Means Clustering**. The objective is to identify distinct customer segments based on demographic information, purchasing behavior, and relationship status to support data-driven marketing strategies.

The project demonstrates the complete data analytics workflow, including cleaning, visualization, dimensionality reduction using PCA, clustering, and cluster evaluation.

---

# 📂 Repository Structure

```text
customer/
│
├── ifood_df.csv
├── Customer.ipynb
└── README.md
```

---

# 📊 Dataset Information

The dataset contains customer demographic details, purchasing behavior, campaign responses, and product spending information.

### Key Features

### Demographics

- Year_Birth
- Income
- Education
- Marital Status
- Kidhome
- Teenhome

### Customer Spending

- MntWines
- MntFruits
- MntMeatProducts
- MntFishProducts
- MntSweetProducts
- MntGoldProds
- MntTotal

### Purchase Channels

- NumWebPurchases
- NumCatalogPurchases
- NumStorePurchases
- NumDealsPurchases
- NumWebVisitsMonth

### Campaign Response

- AcceptedCmp1
- AcceptedCmp2
- AcceptedCmp3
- AcceptedCmp4
- AcceptedCmp5
- Response

### Customer Activity

- Recency
- Customer_Days
- Complain

---

# 🎯 Project Objectives

- Clean and preprocess customer data
- Perform exploratory data analysis
- Engineer meaningful customer features
- Detect and remove outliers
- Analyze customer purchasing behavior
- Visualize customer demographics
- Segment customers using K-Means Clustering
- Evaluate clustering performance
- Visualize customer clusters using PCA

---

# 🧹 Data Preprocessing

The following preprocessing steps are performed:

- Removed duplicate records
- Checked for missing values
- Filled missing Income values using the median
- Removed unnecessary columns:
  - Z_CostContact
  - Z_Revenue
- Created Age from Year_Birth
- Generated new customer features:
  - TotalPurchases
  - FamilySize
  - AvgOrderValue
- Removed spending outliers using the IQR method

---

# ⚙️ Feature Engineering

Several new features were created to improve customer analysis.

### Age

```
Age = 2025 - Year_Birth
```

### Total Purchases

```
TotalPurchases =
NumWebPurchases +
NumCatalogPurchases +
NumStorePurchases
```

### Family Size

```
FamilySize =
Kidhome +
Teenhome
```

### Average Order Value

```
AvgOrderValue =
MntTotal / (TotalPurchases + 1)
```

### Relationship Status

Customers are grouped into:

- In Relationship
- Not In Relationship

based on marital status.

---

# 📈 Exploratory Data Analysis

The project includes multiple visualizations to understand customer behavior.

### Distribution Analysis

- Age Distribution
- Income Distribution
- Total Spending Distribution

### Relationship Analysis

- Income vs Total Spending
- Income vs Total Purchases

### Product Analysis

Average spending on:

- Wines
- Fruits
- Meat Products
- Fish Products
- Sweet Products
- Gold Products

### Purchase Channels

Average purchases through:

- Website
- Catalog
- Physical Store

### Campaign Analysis

Acceptance rate of all marketing campaigns.

### RFM Analysis

Customer behavior analyzed using:

- Recency
- Frequency
- Monetary Value

---

# 📊 Correlation Analysis

A correlation heatmap is generated for:

- Income
- Age
- Family Size
- Total Spending

This helps identify relationships among important customer attributes.

---

# 👥 Customer Segmentation

## Algorithm Used

**K-Means Clustering**

Customer segmentation is performed using:

- Income
- Total Spending
- Relationship Status

---

# 📉 Dimensionality Reduction

**Principal Component Analysis (PCA)** is applied to reduce the clustering features into two principal components for visualization.

---

# 📊 Cluster Evaluation

The project evaluates clustering performance using:

### Elbow Method

Determines the optimal number of clusters by analyzing inertia.

### Silhouette Score

Measures the quality of cluster separation.

---

# 📈 Cluster Visualizations

The project generates:

- Elbow Curve
- Silhouette Score Plot
- Cluster Size Distribution
- PCA Cluster Scatter Plot
- Income by Cluster
- Relationship Status by Cluster

---

# 📊 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

---

# 📚 Python Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler
from sklearn.decomposition import PCA
from sklearn.metrics import silhouette_score

from scipy.stats import pointbiserialr
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/SathwikSL/Data-Analytics.git
```

Navigate to the project folder

```bash
cd Data-Analytics/customer
```

Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
```

---

# ▶️ Running the Project

Launch the Jupyter Notebook:

```bash
jupyter notebook Customer.ipynb
```

---

# 📌 Features

- ✔ Data Cleaning
- ✔ Missing Value Handling
- ✔ Duplicate Removal
- ✔ Feature Engineering
- ✔ Outlier Detection (IQR)
- ✔ Exploratory Data Analysis
- ✔ Correlation Analysis
- ✔ Customer Behavior Analysis
- ✔ RFM Analysis
- ✔ PCA Dimensionality Reduction
- ✔ K-Means Clustering
- ✔ Cluster Evaluation
- ✔ Cluster Visualization

---

# 📂 Project Outputs

The notebook generates:

- Age Distribution
- Income Distribution
- Spending Distribution
- Income vs Spending Scatter Plot
- Product Category Spending
- Purchase Channel Analysis
- Campaign Acceptance Rates
- Correlation Heatmap
- Pair Plot (RFM Analysis)
- Elbow Method Plot
- Silhouette Score Plot
- Cluster Size Chart
- PCA Cluster Visualization
- Income by Cluster
- Relationship Status by Cluster

---

# 🚀 Future Enhancements

- Hierarchical Clustering
- DBSCAN Clustering
- Customer Lifetime Value (CLV) Prediction
- Interactive Dashboard using Streamlit
- Power BI Customer Segmentation Dashboard
- Automated Customer Recommendation System
- Predictive Marketing Models

---

# 🎯 Learning Outcomes

This project demonstrates how to:

- Clean and preprocess customer data
- Engineer meaningful business features
- Perform exploratory data analysis
- Detect statistical outliers
- Evaluate customer purchasing behavior
- Apply K-Means clustering
- Evaluate clustering quality
- Visualize customer segments using PCA

---

# 👨‍💻 Author

**Sathwik S L**

GitHub: https://github.com/SathwikSL

---
