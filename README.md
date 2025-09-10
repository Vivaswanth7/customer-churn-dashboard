📌 Overview

This project focuses on analyzing customer behavior and predicting churn using the Telco Customer Churn dataset.
It combines machine learning for churn prediction with unsupervised clustering for customer segmentation, and presents insights through an interactive dashboard.

📊 Dataset

Source: Kaggle – Telco Customer Churn

Size: ~7,000 customers

Features: Customer demographics, contract details, services, billing and payment information

Target: Churn status (Yes / No)

⚙️ Approach

Data Preprocessing

Cleaned missing values and encoded categorical variables.

Scaled numerical features such as tenure, MonthlyCharges, and TotalCharges.

Churn Prediction

Trained a Random Forest classifier with SMOTE to handle class imbalance.

Optimized the decision threshold (0.29) to maximize the F1-score.

Customer Segmentation

Applied KMeans clustering on tenure and monthly charges.

Identified three main customer segments:

High-risk: short tenure, high charges

Loyal: long tenure, stable charges

Low-value: short tenure, low charges

Dashboard

Built with Streamlit to explore churn predictions and customer clusters interactively.

📈 Results

Churn Recall: ~82% (caught 306 of 374 churners)

Churn Precision: ~49%

F1-score: ~0.62

ROC AUC: ~0.83

Key Insights:

Customers with short tenure, high monthly charges, fiber optic internet, and electronic check payments are most likely to churn.

Two-year contracts and value-added services (like Online Security) significantly reduce churn.

📷 Visuals

ROC Curve


Confusion Matrix


Precision-Recall Curve


Feature Importances


🛠 Tools & Technologies

Python (Pandas, NumPy)

Scikit-learn, imbalanced-learn, XGBoost

Matplotlib, Seaborn, Plotly

Streamlit

Joblib

✍️ Author

Developed by Vivaswanth Sadasivuni
