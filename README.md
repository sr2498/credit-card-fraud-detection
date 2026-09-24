# Credit Card Fraud Detection Using Machine Learning 

A Machine Learning project designed to identify potentially fraudulent credit card transactions using multiple classification algorithms while addressing the challenge of **highly imbalanced transaction data**.

The project covers the complete machine learning workflow, including **Exploratory Data Analysis (EDA), data preprocessing, class balancing with SMOTE, model training, model evaluation, and fraud prediction**.

---

## Project Overview

Credit card fraud detection is a challenging classification problem because fraudulent transactions typically represent only a very small percentage of all transactions.

In this project, multiple supervised machine learning algorithms are trained and evaluated to distinguish between **fraudulent and legitimate transactions**.

Special attention is given to handling **class imbalance** using the **Synthetic Minority Oversampling Technique (SMOTE)** and evaluating models using metrics such as **Precision, Recall, F1-Score, Accuracy, and Confusion Matrix**.


---

## Objectives

The main objectives of this project are to:

- Analyze credit card transaction data and identify patterns related to fraudulent activity.
- Prepare and preprocess transaction data for machine learning.
- Handle highly imbalanced fraud data using **SMOTE**.
- Train multiple classification algorithms.
- Compare model performance using appropriate classification metrics.
- Evaluate the trade-off between detecting fraudulent transactions and minimizing false fraud alerts.
- Build a foundation for a practical fraud detection system.

---

## Technology Stack

| Area | Technologies |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Imbalanced Data Handling | Imbalanced-learn, SMOTE |
| Advanced ML | XGBoost |
| Development Environment | Jupyter Notebook, Google Colab |

---

## Machine Learning Algorithms

The project evaluates multiple classification algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- XGBoost Classifier

Using multiple algorithms makes it possible to compare different approaches and understand which models perform effectively on imbalanced fraud-detection data.

## Project Workflow

```text
Credit Card Transaction Data
            ↓
Exploratory Data Analysis
            ↓
     Data Preprocessing
            ↓
   Train / Test Split
            ↓
Class Imbalance Handling
          (SMOTE)
            ↓
       Model Training
            ↓
      Model Evaluation
            ↓
     Fraud Prediction
```

## Exploratory Data Analysis

Exploratory Data Analysis is performed to better understand the dataset before model training.

The analysis includes:

- Dataset structure and feature inspection
- Missing-value analysis
- Fraud vs. legitimate transaction distribution
- Transaction amount analysis
- Feature distribution analysis
- Correlation analysis
- Visualization of transaction pattern

A major focus of the analysis is understanding the imbalance between fraudulent and legitimate transactions.

---

## Data Preprocessing

Before training the machine learning models, the dataset is prepared through several preprocessing steps.

These include:

- Checking for missing values
- Removing unnecessary features
- Scaling numerical features
- Separating features and target variables
- Splitting data into training and testing datasets
- Applying SMOTE to address class imbalance

---

## Handling Class Imbalance with SMOTE

Fraud detection datasets are commonly **highly imbalanced**, meaning legitimate transactions significantly outnumber fraudulent transactions.

For example:

```text
Legitimate Transactions  ███████████████████████████
Fraud Transactions       █
```
Training directly on highly imbalanced data can cause a model to focus heavily on the majority class.

To address this problem, the project uses **SMOTE (Synthetic Minority Oversampling Technique)**.

SMOTE creates synthetic examples of the minority class based on existing minority-class observations.

```text
Original Training Data
        ↓
Fraud Class = Minority
        ↓
       SMOTE
        ↓
Additional Synthetic Fraud Samples
        ↓
More Balanced Training Data
```

This gives the machine learning models more minority-class examples from which to learn.

> **Important:** SMOTE should be applied only to the training data after the train/test split. The test dataset should remain unchanged so that model evaluation reflects the original data distribution.

---

# Different Machine Learning Models -------------------------------------------------

The following classification models were implemented:

## 1. Logistic Regression

A baseline classification model used to understand linear relationships between features and fraud probability.

---

## 2. K-Nearest Neighbors (KNN)

A distance-based algorithm used for transaction classification based on similarity patterns.

---

## 3. Random Forest Classifier

An ensemble learning method that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

---

## 4. XGBoost Classifier

A gradient boosting algorithm known for high performance on structured datasets and classification problems.

---

# Model Evaluation

Models were evaluated using:

### Accuracy
Measures overall prediction correctness.

### Precision
Measures how many predicted fraud cases were actually fraudulent.

### Recall
Measures how many actual fraud cases were successfully detected.

### F1-Score
Balances precision and recall performance.

### Confusion Matrix
Visualizes correct and incorrect classifications.

---

# How to Run the Project

## Clone Repository

```bash
git clone https://github.com/<your-username>/credit-card-fraud-detection.git
```

Navigate into the project folder:

```bash
cd credit-card-fraud-detection
```

# Key Learnings

- Understanding real-world fraud detection challenges.
- Working with highly imbalanced datasets.
- Applying SMOTE for class balancing.
- Comparing multiple machine learning algorithms.
- Evaluating classification models using appropriate metrics.

---

# Future Improvements

- Deploy the model using Flask/FastAPI.
- Create an interactive fraud monitoring dashboard.
- Implement real-time transaction prediction.
- Use deep learning approaches such as Neural Networks.
- Integrate cloud deployment using AWS.

---
