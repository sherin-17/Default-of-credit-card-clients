# 💳 Credit Card Default Prediction

## 📖 Project Overview
This project predicts whether a customer will default on their credit card payment **next month** using the **Default of Credit Card Clients Dataset** (UCI Machine Learning Repository).  
The goal is to explore the dataset, perform preprocessing and exploratory data analysis (EDA), and build machine learning models to classify default vs non-default clients.  

---

## 🎯 Objectives
- Understand the structure and key features of the dataset.
- Perform **data preprocessing** (handling missing values, outliers, scaling).
- Conduct **Exploratory Data Analysis (EDA)** with visualizations.
- Build and evaluate multiple machine learning models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Gradient Boosting
  - K-Nearest Neighbors (KNN)
- Compare model performance using **Accuracy, F1-score, ROC-AUC**.
- Identify the most important features influencing default behavior.

---

## 📊 Dataset
- **Source**: UCI Machine Learning Repository  
- **Rows**: 30,000 clients  
- **Columns**: 24 (demographics, payment history, bill amounts, payment amounts, target)  
- **Target Variable**: `default payment next month`  
  - `0` → No default  
  - `1` → Default  

---

## 🧹 Data Preprocessing
- Dropped non-predictive column: `ID`
- Handled missing values with median imputation
- Checked for skewness, kurtosis, and outliers (IQR method)
- Standardized numerical features using **StandardScaler**
- Split data into **Train (80%)** and **Test (20%)** with stratified sampling

---

## 📈 Exploratory Data Analysis (EDA)
- Target distribution (imbalanced: ~78% no default, ~22% default)
- Demographics analysis (AGE, SEX, EDUCATION, MARRIAGE)
- Payment history (`PAY_0` to `PAY_6`)
- Distribution of **Bill Amounts** and **Payment Amounts**
- Correlation heatmap
- Outlier detection (boxplots)

---

## 🤖 Model Building
Implemented and evaluated the following models:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- KNN

Each model was trained on scaled training data and tested on unseen data.

---

## 📈 Performance Evaluation
Metrics used:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Visualizations:
- Confusion Matrix
- ROC Curves
- Model Comparison Bar Chart

---

## 🏆 Results
- **Best Performing Model**: *Gradient Boosting* (highest ROC-AUC & F1-score)
- Random Forest also performed strongly
- Logistic Regression gave interpretable feature importance

---

## 🔧 Technologies Used
- Python 🐍
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---


## 📌 Conclusion
- Payment history and bill amounts are strong predictors of default.
- Ensemble models (Random Forest, Gradient Boosting) performed best.
- The project demonstrates a complete pipeline: **EDA → Preprocessing → Modeling → Evaluation**.

---

## 🚀 Future Work
- Handle class imbalance using **SMOTE** or class weights.
- Try advanced models (XGBoost, LightGBM).
- Deploy as a web app (Flask/Streamlit).

---

## ✨ Author
👤 **Shiba sherin**  
📍 Kochi, Kerala, India  
📧 Contact: shibasherin12@gmail.com  


## 📂 Project Structure
