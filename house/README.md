# 🏠 House Price Prediction using Linear Regression

## 📖 Overview

This project develops a **House Price Prediction** model using **Multiple Linear Regression**. The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, feature selection, regression modeling, multicollinearity analysis, and model evaluation.

The objective is to identify the key factors affecting house prices and build a predictive model capable of estimating house prices based on various property features.

---

# 📂 Repository Structure

```text
house/
│
├── Housing.csv
├── housing.ipynb
└── README.md
```

---

# 📊 Dataset Information

The dataset contains residential housing information with attributes describing the physical characteristics and amenities of each house.

### Features

- Price
- Area
- Bedrooms
- Bathrooms
- Stories
- Main Road Access
- Guest Room
- Basement
- Hot Water Heating
- Air Conditioning
- Parking
- Preferred Area
- Furnishing Status

---

# 🎯 Project Objectives

- Explore the housing dataset
- Handle missing values
- Detect and remove outliers
- Encode categorical variables
- Scale numerical features
- Select the most important features
- Train a Multiple Linear Regression model
- Evaluate prediction performance
- Visualize model results

---

# 🧹 Data Preprocessing

The following preprocessing steps are performed:

### ✅ Data Inspection

- Display first five rows
- Dataset shape
- Data types
- Statistical summary

### ✅ Missing Value Analysis

- Checked percentage of missing values
- Verified dataset completeness

### ✅ Outlier Detection

Outliers are detected using:

- Box Plots
- Interquartile Range (IQR)

Outlier treatment is applied to:

- Price
- Area

---

# 📊 Exploratory Data Analysis

The notebook includes several visualizations:

### Numerical Variables

- Pair Plot
- Box Plots

### Categorical Variables

Price comparison based on:

- Main Road Access
- Guest Room
- Basement
- Hot Water Heating
- Air Conditioning
- Furnishing Status

Additional visualization:

- Furnishing Status vs Price
- Air Conditioning comparison

---

# 🔄 Data Transformation

### Binary Encoding

The following columns are converted into binary values:

- Main Road
- Guest Room
- Basement
- Hot Water Heating
- Air Conditioning
- Preferred Area

Example:

```
Yes → 1

No → 0
```

---

### One-Hot Encoding

Dummy variables are created for:

- Furnishing Status

---

# ✂️ Train-Test Split

Dataset split:

- Training Data → 70%
- Testing Data → 30%

Random State:

```
100
```

---

# 📏 Feature Scaling

Numerical features are normalized using:

**MinMaxScaler**

Scaled Features:

- Area
- Bedrooms
- Bathrooms
- Stories
- Parking
- Price

---

# 🔥 Correlation Analysis

A correlation heatmap is generated to visualize relationships among numerical features and identify highly correlated variables.

---

# 🎯 Feature Selection

Recursive Feature Elimination (**RFE**) is used with **Linear Regression** to identify the six most important features contributing to house price prediction.

---

# 📈 Linear Regression Model

A Multiple Linear Regression model is built using **Statsmodels OLS (Ordinary Least Squares)**.

The model summary includes:

- Coefficients
- R² Score
- Adjusted R²
- P-values
- F-statistic
- Confidence Intervals

---

# 📉 Multicollinearity Analysis

Variance Inflation Factor (**VIF**) is calculated to detect multicollinearity among selected features.

The VIF table helps determine whether independent variables are highly correlated.

---

# 📊 Residual Analysis

Residual diagnostics include:

- Residual Distribution Histogram
- Residual Scatter Plot

These plots help validate regression assumptions.

---

# 📈 Model Evaluation

The model is evaluated using:

- R² Score
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

---

# 📉 Prediction Visualization

A scatter plot compares:

- Actual House Prices
- Predicted House Prices

A reference line is included to assess prediction accuracy.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

---

# 📚 Python Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import MinMaxScaler
from sklearn.feature_selection import RFE
from sklearn.linear_model import LinearRegression
from sklearn.metrics import r2_score, mean_squared_error

import statsmodels.api as sm
from statsmodels.stats.outliers_influence import variance_inflation_factor
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/SathwikSL/Data-Analytics.git
```

Navigate to the project directory:

```bash
cd Data-Analytics/house
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

---

# ▶️ Running the Project

Launch the notebook:

```bash
jupyter notebook housing.ipynb
```

---

# 📌 Features

- ✔ Data Inspection
- ✔ Missing Value Analysis
- ✔ Outlier Detection
- ✔ Exploratory Data Analysis
- ✔ Binary Encoding
- ✔ One-Hot Encoding
- ✔ Feature Scaling
- ✔ Correlation Analysis
- ✔ Feature Selection (RFE)
- ✔ Multiple Linear Regression
- ✔ VIF Analysis
- ✔ Residual Analysis
- ✔ Model Evaluation
- ✔ House Price Prediction

---

# 📂 Project Outputs

The notebook generates:

- Pair Plot
- Box Plots
- Correlation Heatmap
- Selected Features
- OLS Regression Summary
- VIF Table
- Residual Distribution Plot
- Residual Scatter Plot
- Actual vs Predicted House Price Plot
- Model Performance Metrics

---

# 📊 Performance Metrics

The regression model is evaluated using:

- **R² Score** – Measures how well the model explains the variance in house prices.
- **Mean Squared Error (MSE)** – Measures the average squared prediction error.
- **Root Mean Squared Error (RMSE)** – Represents the average prediction error in the original price scale.

---

# 🚀 Future Enhancements

- Ridge Regression
- Lasso Regression
- Elastic Net Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor
- Hyperparameter Tuning
- Interactive Streamlit Web Application
- House Price Prediction Dashboard using Power BI

---

# 🎯 Learning Outcomes

This project demonstrates how to:

- Perform data preprocessing for regression problems
- Detect and remove outliers
- Encode categorical variables
- Normalize numerical features
- Select important features using RFE
- Build and interpret a Multiple Linear Regression model
- Analyze multicollinearity using VIF
- Evaluate regression performance
- Visualize prediction accuracy

---

# 👨‍💻 Author

**Sathwik S L**

GitHub: https://github.com/SathwikSL

---
