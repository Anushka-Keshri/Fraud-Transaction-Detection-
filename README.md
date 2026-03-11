# Credit Card Fraud Detection using Machine Learning

## Overview

Credit card fraud detection is a critical problem in financial systems because fraudulent transactions are extremely rare compared to legitimate transactions. This project builds a machine learning system to identify fraudulent credit card transactions using classification models and explainable AI techniques.

The goal of the project is to detect fraud with high recall while minimizing false positives. Multiple machine learning models were trained and compared, and the best-performing model was analyzed using SHAP explainability.

---

## Dataset

Dataset used: **Credit Card Fraud Detection Dataset**

* Total transactions: **284,807**
* Fraudulent transactions: **492**
* Fraud rate: **~0.17%**

The dataset contains anonymized numerical features (V1–V28) obtained using PCA transformation, along with transaction **Amount** and **Time**.

Target variable:

* **Class = 0 → Normal Transaction**
* **Class = 1 → Fraud Transaction**

---

## Project Workflow

1. Data Loading
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
4. Handling Class Imbalance
5. Model Training
6. Model Evaluation
7. Model Comparison
8. Feature Importance Analysis
9. Model Explainability using SHAP

---

## Exploratory Data Analysis

Key observations:

* Fraud transactions represent **less than 0.2%** of the dataset.
* The dataset is extremely **imbalanced**, making accuracy an unreliable metric.
* Fraud detection requires focusing on **recall, precision, and ROC-AUC** instead of accuracy.

---

## Machine Learning Models Used

The following classification models were trained and evaluated:

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

These models were compared to determine the best-performing approach for fraud detection.

---

## Evaluation Metrics

Because the dataset is highly imbalanced, the following evaluation metrics were used:

* **Precision** – percentage of predicted fraud transactions that were actually fraud
* **Recall** – percentage of fraud transactions successfully detected
* **F1 Score** – harmonic mean of precision and recall
* **ROC-AUC Score** – ability of the model to separate fraud and normal transactions

Accuracy alone is misleading in fraud detection tasks.

---

## Model Performance

| Model               | Recall   | Precision | ROC-AUC  |
| ------------------- | -------- | --------- | -------- |
| Logistic Regression |          |           |          |
| Random Forest       |          |           |          |
| XGBoost             | **0.87** | **0.51**  | **0.97** |

*(Replace missing values with your computed results if needed)*

---

## Feature Importance

Feature importance analysis was performed to identify which variables contribute the most to fraud detection. Tree-based models such as Random Forest and XGBoost provide importance scores that indicate how strongly each feature influences predictions.

---

## Model Explainability (SHAP)

Model explainability was implemented using **SHAP (SHapley Additive exPlanations)**.

SHAP helps interpret how individual features contribute to model predictions. This is important in financial systems where model transparency is required.

SHAP analysis provides:

* Global feature importance
* Local explanations for individual predictions
* Visualization of feature impact on fraud detection

Example visualization:

```
SHAP summary plots show how different features push predictions toward fraud or non-fraud.
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* SHAP (Explainable AI)
* Matplotlib
* Seaborn
* Google Colab

---

## Project Structure

```
fraud-detection
│
├── fraud_detection.ipynb
├── README.md
├── requirements.txt
└── images
```

---

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
```

2. Install required libraries

```bash
pip install -r requirements.txt
```

3. Open the notebook in **Google Colab** or **Jupyter Notebook**

4. Run all cells to reproduce the analysis and model results.

---

## Key Results

* XGBoost achieved the best performance among the evaluated models.
* Fraud detection recall reached **~87%**, meaning most fraudulent transactions were successfully identified.
* ROC-AUC score of **~0.97** indicates strong classification capability.
* SHAP explainability provides insights into the factors influencing fraud predictions.

---

## Future Improvements

Possible improvements for this project include:

* Hyperparameter tuning for improved model performance
* Real-time fraud detection systems
* Advanced anomaly detection methods
* Deployment using APIs or dashboards

---

## Author

**Anushka Keshri**

Machine Learning and Data Analytics Enthusiast

