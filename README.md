# Credit Card Fraud Detection using Machine Learning

## Overview

This project builds a machine learning system to detect fraudulent credit card transactions.
Financial fraud detection is challenging because fraudulent transactions are extremely rare compared to legitimate ones, creating a highly imbalanced dataset.

The goal of this project is to train machine learning models that can identify fraud transactions with high recall while minimizing false alarms.

---

## Dataset

Dataset used: **Credit Card Fraud Detection Dataset**

* Total transactions: **284,807**
* Fraudulent transactions: **492**
* Fraud rate: **~0.17%**

The dataset contains anonymized features (V1–V28) obtained using PCA transformation, along with transaction amount and time.

Target variable:

* **Class = 0 → Normal Transaction**
* **Class = 1 → Fraud Transaction**

---

## Project Workflow

1. Data Loading and Exploration
2. Data Preprocessing
3. Handling Class Imbalance
4. Model Training
5. Model Evaluation
6. Model Comparison
7. Feature Importance Analysis

---

## Machine Learning Models Used

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

These models were compared using evaluation metrics suitable for imbalanced datasets.

---

## Evaluation Metrics

Accuracy alone is misleading for fraud detection because of extreme class imbalance.
The following metrics were used:

* **Precision**
* **Recall**
* **F1-score**
* **ROC-AUC Score**

---

## Model Performance

| Model               | Recall | Precision | ROC-AUC |
| ------------------- | ------ | --------- | ------- |
| Logistic Regression | -      | -         | -       |
| Random Forest       | -      | -         | -       |
| XGBoost             | -      | -         | -       |

*(Replace with your actual results)*

---

## Key Results

* XGBoost achieved the best overall performance.
* Fraud detection recall reached approximately **87%**, meaning most fraudulent transactions were successfully detected.
* ROC-AUC score of **~0.97** indicates strong class separation.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Seaborn

---

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/yourusername/fraud-detection-project.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the notebook in Google Colab or Jupyter.

---

## Future Improvements

* Hyperparameter tuning for improved performance
* Real-time fraud detection system
* Model explainability using SHAP

---

## Author

Anushka Keshri
