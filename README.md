# 💳 Credit Card Fraud Detection

## 📌 Project Overview
This project analyzes a **credit card transactions dataset** (from Kaggle) to detect fraudulent activities.  
It demonstrates skills in **data cleaning, exploratory data analysis (EDA), feature engineering, and handling imbalanced datasets**.  
I also implemented baseline ML models (Logistic Regression, Random Forest) to evaluate fraud detection performance.

---

## 🚀 Workflow
1. **Data Cleaning & Preprocessing**
   - Removed duplicates, checked missing values
   - Scaled `Amount`, created `Hour` feature from `Time`
   - Bucketized `Amount` into ranges (small/medium/large)

2. **Exploratory Data Analysis (EDA)**
   - Class distribution (fraud vs. non-fraud)
   - Amount distribution by fraud status
   - Transactions by hour of the day
   - Correlation analysis of features with fraud

3. **Feature Engineering**
   - Created time-based and bucketized features
   - Prepared dataset for modeling

4. **Modeling**
   - Logistic Regression (with class weights)
   - Random Forest (with class weights)
   - ROC-AUC and classification reports

5. **Visualization**
   - Fraud distribution  
   - Amount vs Class (log scale)  
   - Transactions by Hour  
   - Top features correlated with fraud  
   - ROC curves  

---

## 📂 Files
- `fraud_detection.ipynb` → Jupyter Notebook (full workflow)  
- `cleaned_creditcard.csv` → Preprocessed dataset  
- Plots:  
  - `class_distribution.png`  
  - `amount_distribution_by_class.png`  
  - `transactions_by_hour.png`  
  - `top_corr_with_class.png`  
  - `roc_curves.png`  
- `metrics.json` → Model evaluation metrics  

---

## 📈 Key Insights
- Fraud transactions make up only **0.17%** of total → highly imbalanced dataset.  
- Fraud amounts are often **smaller and frequent**, not always large.  
- Certain hours of the day show higher fraud frequency.  
- Logistic Regression and Random Forest achieved strong **ROC-AUC scores (>0.95)**.  

---

## 🛠 Tools & Technologies
- **Python** → Pandas, NumPy, Scikit-learn  
- **Visualization** → Matplotlib, Seaborn  
- **ML Models** → Logistic Regression, Random Forest  
- **Imbalanced Data Handling** → Class weights, SMOTE (optional)  
- **Version Control** → GitHub  

---

## 📌 Future Improvements
- Try advanced ML models (XGBoost, LightGBM).  
- Deploy model as API / dashboard.  
- Automate data pipeline for fraud monitoring.  

---

