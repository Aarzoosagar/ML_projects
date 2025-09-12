Fraud Detection with LightGBM

📌 Overview

This project builds a fraud detection model using LightGBM, applied on the Fraud.csv dataset.
It demonstrates the full data science pipeline, from data cleaning to business recommendations.

Candidate Expectations Covered
Data cleaning – missing values, outliers, multicollinearity
Fraud detection model – detailed explanation of LightGBM
Variable selection – VIF check & feature importance
Model performance – Confusion Matrix, ROC-AUC, PR-AUC
Key fraud factors – extracted from feature importance
Interpretation – do these factors make sense?
Prevention strategy – business recommendations for companies
Monitoring – how to evaluate if actions are working




Dependencies include:
pandas, numpy
scikit-learn
lightgbm
statsmodels
matplotlib, seaborn
joblib

▶️ Usage
Option 1 – Jupyter Notebook
Run the full pipeline step by step:
jupyter notebook notebooks/Fraud_Detection.ipynb
Option 2 – Python Scripts
Run modular scripts from src/:
data_preprocessing.py → handles missing values, outliers, encoding, multicollinearity
model_training.py → trains and evaluates LightGBM model
feature_analysis.py → shows feature importance and key fraud factors
recommendations.py → outputs business strategies

📊 Results

Confusion Matrix & Classification Report
ROC-AUC Score for model evaluation
PR-AUC Score to handle imbalance
Feature Importance Chart – top predictors of fraud

🔑 Business Insights

Large/unusual transaction amounts are strong fraud indicators.
New or unusual merchants/devices increase fraud risk.
Velocity (too many transactions in short time) is suspicious.

🛡️ Recommendations

Enable real-time alerts for suspicious transactions.
Enforce multi-factor authentication for high-risk transactions.
Set adaptive transaction limits for new customers.
Retrain the model periodically with new fraud patterns.

📈 Monitoring Effectiveness

Compare fraud rate before vs after interventions.
Track false positives (legit users wrongly flagged).
Monitor metrics over time: Precision, Recall, ROC-AUC, PR-AUC.
Use A/B testing to validate prevention strategies.
