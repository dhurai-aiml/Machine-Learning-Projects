# 🏠 Chennai House Price Prediction using Machine Learning

A machine learning regression project that predicts house sale prices in Chennai based on property features like area, size, location, and amenities. The project includes full data preprocessing, feature engineering, model training, and evaluation using multiple ML algorithms.

---

## 📌 Project Overview

This project builds a supervised machine learning system to estimate real estate prices in Chennai using historical housing data. It includes end-to-end steps from raw data cleaning to model comparison, ensuring accurate and data-driven price prediction.

The goal is to help users estimate property prices based on key housing attributes and improve decision-making in real estate investments.

---

## 🧰 Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, SciPy
- **ML Models:** Linear Regression, Decision Tree, Random Forest, SVR, KNN
- **Preprocessing:** Label Encoding, StandardScaler
- **Evaluation Metrics:** R² Score, MAE, RMSE

---

## 📁 Dataset Overview

Dataset: Chennai_housing_sale.csv
Shape: 7109 rows × 19 columns

**Key Features:**

- Area (Location in Chennai)
- INT_SQFT (Interior Sq. Ft)
- N_BEDROOM, N_BATHROOM, N_ROOM
- SALE_COND, BUILDTYPE, STREET, MZZONE
- PARK_FACIL, UTILITY_AVAIL
- COMMIS (Commission)
- SALES_PRICE (Target variable)

---

## 🔄 Workflow Summary

### 1. Data Loading & Inspection
Loaded dataset using Pandas
Checked structure, null values, and statistics

### 2. Data Cleaning
Handled missing values:
Mean imputation for numerical features
Fixed inconsistent categorical labels (e.g., "Adj Land" → "AdjLand")
Removed redundant columns:
QS_ROOMS, QS_BATHROOM, QS_BEDROOM, QS_OVERALL, DIST_MAINROAD

### 3. Exploratory Data Analysis (EDA)
Distribution plots for numeric features
Boxplots for outlier detection
Correlation heatmap for feature relationships

### 4. Feature Selection
Used correlation analysis + ANOVA test
Selected features strongly related to SALES_PRICE

### 5. Encoding Categorical Data
Applied Label Encoding to all categorical columns

### 6. Train-Test Split
80% Training data
20% Testing data

### 7. Feature Scaling
Applied StandardScaler for normalization

### 8. Model Building

Trained multiple regression models:

Linear Regression,
Decision Tree Regressor,
Random Forest Regressor,
Support Vector Regressor (SVR),
K-Nearest Neighbors Regressor

---

## 📊 Model Performance

| Model             | Training R² | Testing R² |
| ----------------- | ----------- | ---------- |
| Linear Regression | 0.8114      | 0.8078     |
| Decision Tree     | 1.0000      | 0.9584     |
| SVR               | -0.0207     | -0.0142    |
| KNN               | 0.9178      | 0.8631     |
| Random Forest     | 0.9974      | **0.9813** |

---

## 🏆 Best Model
### 👉 Random Forest Regressor
- Highest accuracy on test data: 98.13%
- Best balance between bias and variance
- Strong generalization performance

---

## 🚀 How to Run
## ⚙️ Setup

1. Clone the repo
```bash
git clone https://github.com/dhurai-aiml/chennai-house-price-prediction.git
cd chennai-house-price-prediction
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Run notebook / script
```
python train.py
```
---

## 🧑‍💻 Author

**Dhurai Murugan S** — Fresher | AIML & Gen AI Enthusiast

**Skills:** Python • Machine Learning • Deep Learning • NLP • Generative AI • RAG Systems • Agentic AI

[LinkedIn](https://linkedin.com/in/yourprofile) • [GitHub](https://github.com/dhurai-aiml)
