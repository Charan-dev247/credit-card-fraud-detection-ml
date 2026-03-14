# Credit Card Fraud Detection using Machine Learning

## Overview
Credit card fraud detection is a critical problem in financial systems. Fraudulent transactions represent only a tiny fraction of all transactions, making the dataset highly imbalanced and the detection task challenging.

This project applies machine learning techniques to identify fraudulent credit card transactions using a real-world dataset.

---

## Dataset

The dataset contains credit card transactions made by European cardholders in September 2013.

Key statistics:

- **Total transactions:** 284,807  
- **Fraudulent transactions:** 492  
- **Fraud percentage:** ~0.17%

Due to privacy concerns, the original transaction features are not available. Instead, the dataset contains **28 anonymized features obtained using Principal Component Analysis (PCA).**

### Important Features

| Feature | Description |
|------|-------------|
| Time | Seconds elapsed between the transaction and the first transaction |
| V1 – V28 | PCA-transformed features |
| Amount | Transaction amount |
| Class | Target variable (0 = normal, 1 = fraud) |

---

## Problem Statement

Fraud detection is a **binary classification problem** where the goal is to identify whether a transaction is legitimate or fraudulent.

The major challenge is **class imbalance**, since fraudulent transactions represent only a very small portion of the dataset.

---

## Machine Learning Models Used

The following models were implemented and compared:

- **Logistic Regression**
- **Random Forest Classifier**

These models were trained and evaluated to determine their ability to detect fraudulent transactions.

---

## Evaluation Metrics

Because the dataset is highly imbalanced, accuracy alone is not a reliable metric.

The following evaluation metrics were used:

- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC**

These metrics provide better insight into the model's ability to detect rare fraud cases.

---

## Results

The Random Forest model achieved better performance compared to Logistic Regression in detecting fraudulent transactions.

The results indicate that ensemble learning methods can capture complex patterns in fraud detection tasks.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

credit-card-fraud-detection-ml
│
├── notebooks
│ └── fraud_detection.ipynb
│
├── images
│
├── README.md
├── requirements.txt
└── .gitignore


---

## Future Improvements

Possible improvements for this project include:

- Using **SMOTE** for handling class imbalance
- Trying **Gradient Boosting models (XGBoost / LightGBM)**
- Applying **Deep Learning methods**
- Deploying the model as a **real-time fraud detection system**

---

## Author

**Suluru Charan**  
B.Tech CSE (AI)  
IIITDM Kancheepuram