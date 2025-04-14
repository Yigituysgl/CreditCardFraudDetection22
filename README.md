# CreditCardFraudDetection22
Credit Card Fraud Detection with Machine Learning
Project Description:

This project detects "credit card fraud" using powerful machine learning algorithms trained on real-world anonymized transactions.  
Built as part of my portfolio to demonstrate:
- Real-world ML pipeline
- Handling imbalanced data
- Model comparison & evaluation

- Goal: Accurately identify tricky transactions while minimizing false alarms.

- 📂 Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Rows: 284,807 transactions  
- Features: V1–V28 (PCA transformed), `Amount`, `Time`, and `Class` (0 = normal, 1 = fraud)

- ML Workflow

1. Data Cleaning & Exploration
2. Feature Scaling (`StandardScaler`)
3. Handling Imbalanced Classes (`SMOTE` + `scale_pos_weight`)
4. Train-Test Split (Stratified)
5. Train 3 Models:
   - Logistic Regression
   - Random Forest
   - XGBoost
6. Evaluate using:
   - Classification Report
   - Confusion Matrix
   - ROC Curve + AUC
7. Model Comparison Visualization

Algorithms Compared

| Model               | Precision | Recall | F1-score | AUC  |
|---------------------|-----------|--------|----------|------|
| Logistic Regression | 0.06      | 0.92   | 0.12     | 0.97 |
| Random Forest       | 0.15      | 0.89   | 0.25     | 0.98 |
| XGBoost             |   0.24    | 0.89   | 0.38     | 0.98 |

>  XGBoost wins overall with best F1 and lowest false positives!

Visuals:

- Grouped bar chart: Precision, Recall, F1, AUC per model
- Confusion matrices per model
- ROC curves per model
