# 🛰️ Satellite Health Prediction - Machine Learning Project

This project aims to predict the **health status of satellites** using telemetry data. The process includes data cleaning, exploratory data analysis, and building multiple machine learning models to perform classification. The goal is to classify whether a satellite is in **good** or **bad** health.

---


---

## 📌 Problem Statement

Given a dataset of satellite telemetry data (like temperature, voltage, etc.), predict whether a satellite is in **good** (0) or **bad** (1) health.

---

## 🛠️ Technologies Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (sklearn)

---

## ✅ Project Steps

### 1. Data Loading
- Read the CSV dataset using pandas

### 2. Data Cleaning
- Handle missing values using median imputation
- Drop duplicates
- Cap outliers at the 99th percentile to reduce noise (visualized with box plots)

### 3. Data Analysis & Visualization
- Heatmap for correlation analysis
- Box plots for outlier visualization
- Distribution plots for feature understanding
- Feature importance from Random Forest

### 4. Feature Engineering
- Split into independent (X) and dependent (y) variables
- Train-test split (80:20)
- StandardScaler used for feature scaling

### 5. Model Building
Four models were trained and evaluated:
- Logistic Regression
- Random Forest Classifier
- Support Vector Classifier (SVC)
- SGD Classifier

Each model was evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report

### 6. Cross-Validation
- Applied 5-fold cross-validation to evaluate generalization performance.


---

## 📊 Results

- Accuracy Comparison across models displayed using bar chart
- Feature importance shown for better interpretability
- SGDClassifier and RandomForest performed the best in most cases

---

## 📈 Future Improvements

- Real Time Predictions based on inputs.
- Deploy via Streamlit or Flask for UI-based input
- Save models with joblib or pickle
- Use advanced models like XGBoost
- Add hyperparameter tuning (GridSearchCV)



