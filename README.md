# ensembled_model_credit_card_fraud_detection
# 📄 Overview
This project addresses the challenge of detecting credit card fraud using an ensemble-based machine learning framework. It demonstrates how one-class classification and ensemble methods can effectively handle extreme class imbalance and improve fraud detection accuracy in real-world financial datasets.

# 📊 Dataset
Source: Kaggle - Credit Card Fraud Detection

Contains 284,807 transactions, with only 492 (~0.17%) being fraudulent

PCA-transformed features, with 'Time' and 'Amount' retained as original

# 🧠 Methodology
The ensemble model consists of three stages:

SVM (Normal Transactions) — Identifies clear non-fraud transactions

SVM (Fraudulent Transactions) — Detects obvious fraud patterns

Random Forest — Classifies ambiguous ("grey-area") transactions

This design minimizes false positives and optimizes classification accuracy.

# 📈 Results
Metric	Ensemble Model	Isolation Forest
Accuracy	Higher (+0.2%)	-
Precision	0.90	0.26
Recall	0.71	0.27
F1-Score	0.79	0.26
The ensemble method outperformed all standalone models tested.

# 🛠 Models Used
One-Class SVM

Random Forest

Isolation Forest (for comparison)

Local Outlier Factor (LOF)

# 🔍 Exploratory Data Insights
Fraudulent transactions had higher average amounts but showed high variability

Both fraud and normal distributions were right-skewed

Quarter of all fraud cases involved less than $1

# 📌 Key Contributions
Strategic three-stage ensemble for class imbalance

Enhanced precision and reduced false alarms

Demonstrated reproducibility with real-world transaction data
