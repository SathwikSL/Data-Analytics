# 🧹 Data Cleaning Using Python

## 📖 Overview

This project demonstrates essential **Data Cleaning and Preprocessing** techniques using Python on two real-world datasets:

- **Airbnb New York City Listings (AB_NYC_2019.csv)**
- **Canada YouTube Trending Videos (CAvideos.csv)**

The primary objective is to improve data quality by handling missing values, removing duplicate records, correcting data types, detecting outliers, validating data integrity, and exporting cleaned datasets for further analysis or machine learning applications.

---

# 📂 Repository Structure

```text
cleaning/
│
├── AB_NYC_2019.csv
├── AB_NYC_2019_Cleaned.csv
├── CAvideos.csv
├── CAvideos_cleaned.csv
├── Cleaning.ipynb
└── README.md
```

---

# 📊 Datasets

## 1. Airbnb New York City Dataset

The dataset contains Airbnb listing information including:

- Listing Name
- Host Name
- Neighbourhood
- Room Type
- Price
- Minimum Nights
- Number of Reviews
- Reviews Per Month
- Last Review Date
- Availability (365 days)

---

## 2. Canada YouTube Trending Videos Dataset

The dataset contains trending YouTube videos in Canada with features such as:

- Video Title
- Channel Title
- Publish Time
- Views
- Likes
- Dislikes
- Comment Count
- Category ID
- Description

---

# 🎯 Project Objectives

- Load datasets using Pandas
- Handle missing values
- Remove duplicate records
- Standardize data types
- Detect and remove outliers
- Validate data quality
- Export cleaned datasets

---

# 🧹 Data Cleaning Process

## Airbnb Dataset

### ✅ Missing Value Handling

The following missing values are handled:

| Column | Action |
|---------|--------|
| reviews_per_month | Filled with **0** |
| name | Filled with **"Unknown"** |
| host_name | Filled with **"Unknown"** |
| last_review | Converted to DateTime and missing values replaced with **1900-01-01** |

---

### ✅ Duplicate Records

- Checked duplicate records
- Removed duplicate rows

---

### ✅ Data Type Standardization

Converted:

- `last_review` → DateTime

---

### ✅ Outlier Detection

Outliers in the **Price** column are detected using the **Interquartile Range (IQR)** method.

```
IQR = Q3 − Q1

Lower Limit = Q1 − 1.5 × IQR

Upper Limit = Q3 + 1.5 × IQR
```

Records outside the acceptable range are removed.

---

### ✅ Data Validation

The dataset is validated by checking:

- Price greater than zero
- Minimum Nights greater than zero
- Availability not exceeding 365 days

---

### ✅ Output

The cleaned dataset is saved as:

```
AB_NYC_2019_Cleaned.csv
```

---

# 🧹 Canada YouTube Dataset

### ✅ Missing Value Handling

Missing values in the **Description** column are replaced with:

```
No Description Available
```

---

### ✅ Duplicate Removal

- Checked duplicate rows
- Removed duplicate records
- Verified duplicate Video IDs

---

### ✅ Data Type Standardization

Converted:

- Publish Time → DateTime
- Category ID → Integer

Trimmed extra spaces from:

- Video Title
- Channel Title

---

### ✅ Outlier Detection

Outliers in the **Views** column are detected using the **IQR Method**.

A Box Plot is generated to visualize outliers before removing them.

---

### ✅ Output

The cleaned dataset is saved as:

```
CAvideos_cleaned.csv
```

---

# 📈 Visualizations

The project generates the following visualization:

- Box Plot for detecting outliers in the Views column

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib

---

# 📚 Python Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/SathwikSL/Data-Analytics.git
```

Navigate to the project folder:

```bash
cd Data-Analytics/cleaning
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib
```

---

# ▶️ Running the Project

Open the notebook using Jupyter:

```bash
jupyter notebook Cleaning.ipynb
```

or run the Python script if available.

---

# 📌 Features

- ✔ Missing Value Treatment
- ✔ Duplicate Record Removal
- ✔ Data Type Conversion
- ✔ Date Formatting
- ✔ String Cleaning
- ✔ Outlier Detection (IQR Method)
- ✔ Data Integrity Validation
- ✔ Data Export
- ✔ Data Visualization

---

# 📚 Learning Outcomes

This project demonstrates how to:

- Import and inspect datasets
- Handle missing values effectively
- Remove duplicate records
- Standardize inconsistent data
- Detect statistical outliers
- Validate dataset quality
- Prepare datasets for analytics and machine learning

---

# 📂 Output Files

After running the notebook, the following cleaned datasets are generated:

- **AB_NYC_2019_Cleaned.csv**
- **CAvideos_cleaned.csv**

---

# 🚀 Future Enhancements

- Automate data cleaning using reusable functions
- Generate automated data quality reports
- Add interactive dashboards using Streamlit
- Integrate with Power BI
- Build a reusable ETL pipeline

---

# 👨‍💻 Author

**Sathwik S L**

GitHub: https://github.com/SathwikSL

---
