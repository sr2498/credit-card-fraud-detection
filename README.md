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
## Model Development

### 1. Logistic Regression

Logistic Regression is used as a baseline classification model for predicting the probability that a transaction belongs to the fraud class.

It provides a useful starting point for comparing more complex machine learning algorithms.

---

### 2. K-Nearest Neighbors (KNN)

KNN classifies transactions based on their similarity to nearby observations in the feature space.

Feature scaling is particularly important for distance-based algorithms such as KNN.

---

### 3. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines predictions from multiple decision trees.

It can capture nonlinear relationships and complex interactions between transaction features.

---

### 4. XGBoost Classifier

XGBoost is a gradient-boosting algorithm commonly used for structured/tabular machine learning problems.

The model builds trees sequentially, with each new tree attempting to improve errors made by previous trees.

---

## Model Evaluation

Because fraud detection involves highly imbalanced data, **accuracy alone is not sufficient** for evaluating model performance.

The following metrics are considered:

### Precision

Precision measures how many transactions predicted as fraud were actually fraudulent.

```text
High Precision → Fewer false fraud alerts
```

---

### Recall

Recall measures how many actual fraudulent transactions were successfully identified.

```text
High Recall → More fraudulent transactions detected
```

Recall is particularly important in fraud detection because failing to identify a fraudulent transaction can have significant consequences.

---

### F1-Score

F1-Score provides a balance between **Precision and Recall**.

It is useful when both false positives and false negatives need to be considered.

---

### Accuracy

Accuracy measures the percentage of all transactions classified correctly.

However, accuracy should be interpreted carefully for highly imbalanced datasets.

For example, if almost all transactions are legitimate, a model could achieve high accuracy simply by predicting most transactions as legitimate while still missing important fraud cases.

---

### Confusion Matrix

The confusion matrix provides a detailed breakdown of model predictions:

| | Predicted Legitimate | Predicted Fraud |
|---|---:|---:|
| **Actual Legitimate** | True Negative | False Positive |
| **Actual Fraud** | False Negative | True Positive |

For fraud detection:

- **True Positive (TP):** Fraud correctly detected
- **True Negative (TN):** Legitimate transaction correctly identified
- **False Positive (FP):** Legitimate transaction incorrectly flagged as fraud
- **False Negative (FN):** Fraudulent transaction incorrectly classified as legitimate

Reducing **False Negatives** is particularly important when the goal is to detect as many fraudulent transactions as possible.

---

## Model Comparison

The trained models can be compared using:

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | — | — | — | — |
| K-Nearest Neighbors | — | — | — | — |
| Random Forest | — | — | — | — |
| XGBoost | — | — | — | — |

> Replace the placeholders with the actual results generated by the project.

The preferred model should be selected based on the requirements of the fraud-detection use case rather than accuracy alone.

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/credit-card-fraud-detection.git
```

### 2. Navigate to the Project

```bash
cd credit-card-fraud-detection
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn xgboost
```

### 4. Open the Notebook

Run the project using:

- Jupyter Notebook

or

- Google Colab

Then execute the notebook cells sequentially to perform data analysis, preprocessing, model training, and evaluation.

---

## Key Learnings

This project demonstrates practical experience with:

**Data Analysis**
- Data exploration
- Missing-value analysis
- Feature analysis
- Data visualization

**Machine Learning**
- Binary classification
- Model training
- Model comparison
- Fraud prediction

**Imbalanced Data**
- Understanding class imbalance
- Applying SMOTE
- Evaluating minority-class performance

**Model Evaluation**
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

**Python Development**
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- XGBoost
- Imbalanced-learn

---

## Future Enhancements

Potential improvements to the project include:

- Add ROC-AUC and Precision-Recall curve analysis.
- Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Compare SMOTE with class-weight-based approaches.
- Add feature importance analysis.
- Build a REST API using Flask or FastAPI for model inference.
- Create an interactive fraud-monitoring dashboard.
- Add real-time transaction prediction.
- Experiment with additional machine learning and deep learning approaches.
- Containerize the prediction service using Docker.
- Deploy the application to AWS.

---

## Project Purpose

This project demonstrates an end-to-end **machine learning classification workflow for credit card fraud detection**.

It highlights practical experience with **Python, data preprocessing, exploratory data analysis, imbalanced datasets, SMOTE, classification algorithms, model evaluation, and fraud prediction** while demonstrating how machine learning can be applied to a financial-services use case.

