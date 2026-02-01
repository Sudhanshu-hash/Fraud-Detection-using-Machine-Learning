# Fraud-Detection-using-Machine-Learning
This project focuses on building a machine learning model to detect fraudulent financial transactions using historical transaction data. The objective is to identify suspicious transactions and provide insights that can help organizations reduce financial fraud.

# Amazon-Sales-Data-Analysis-Visualization

Goal: To build a machine learning–based fraud detection system that identifies fraudulent financial transactions by analyzing transaction behavior, balance changes, and transaction types, and to derive actionable fraud prevention insights.

1. Data Source and Cleaning:

Source: Financial transaction dataset provided as part of the Accredian Data Science assignment.


Initial Data: Raw transaction data stored in ***Fraud.csv*** containing transaction details such as amount, type, balances, and fraud labels.

Understanding:
Each row represents a single transaction. The dataset includes both normal and fraudulent transactions, with a highly imbalanced target variable (isFraud).

---
2. Data Cleaning and Preprocessing

Purpose:
To ensure data quality and prepare features for machine learning.

Steps Performed:

Checked for missing values across all columns (no major missing values found).

Analyzed outliers in transaction amounts and balance-related features using descriptive statistics.

Examined multicollinearity among balance variables using correlation analysis.

Removed identifier columns (nameOrig, nameDest) as they do not contribute to prediction.

Encoded the categorical type column into numerical form for model compatibility.

---
3. Feature Selection and Dataset Preparation

Logic:
Relevant transaction-related features were selected based on domain knowledge and fraud behavior patterns.

Final Features Included:

Transaction amount

Transaction type (encoded)

Sender and receiver balance information

The target variable (isFraud) was separated, and the dataset was split into training and testing sets using an 80–20 ratio.
---
4. ***Model Development and Evaluation***

Model Used:
Logistic Regression (Supervised Classification)

Reason for Selection:

Suitable for binary classification

Interpretable and efficient

Works well as a baseline fraud detection model

Evaluation Metrics:

Confusion Matrix

Precision

Recall

F1-score

Key Focus:
Recall was prioritized due to the imbalanced nature of fraud data, ensuring that fraudulent transactions are not missed.

---
5. ***Key Insights***

Fraudulent transactions often involve unusually high transaction amounts.

Sudden reductions in sender balances combined with increases in receiver balances are strong fraud indicators.

Transaction type plays a significant role in identifying fraud.

Accuracy alone is insufficient; recall is a more meaningful metric in fraud detection.

---
6. ***Fraud Prevention Recommendations***

Implement real-time transaction monitoring systems.

Apply transaction limits for suspicious activities.

Use multi-factor authentication for sensitive transactions.

Continuously retrain machine learning models to adapt to evolving fraud patterns.

---
7. ***Conclusion***

This project demonstrates an end-to-end machine learning workflow for fraud detection, covering data cleaning, feature selection, model training, evaluation, and interpretation. The approach provides a practical foundation for deploying data-driven fraud prevention systems in real-world financial environments.

---
5. ***Connect with Me***

If you have any questions about this project, want to discuss data strategy, or are interested in collaboration, feel free to connect!
