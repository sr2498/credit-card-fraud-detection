# Credit Card Fraud Detection Using Machine Learning

## 📌 Project Overview

Credit card fraud is a major challenge in the financial industry due to the increasing number of digital transactions. This project focuses on building a machine learning-based fraud detection system that identifies fraudulent credit card transactions while handling highly imbalanced datasets.

The project applies multiple classification algorithms and compares their performance using evaluation metrics such as Precision, Recall, F1-Score, and Accuracy.

---

## 🎯 Objectives

- Detect fraudulent credit card transactions using machine learning models.
- Handle class imbalance using Synthetic Minority Oversampling Technique (SMOTE).
- Perform data preprocessing and exploratory data analysis.
- Train and evaluate multiple classification models.
- Identify the best-performing model for fraud prediction.

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Libraries & Frameworks
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

### Machine Learning Algorithms
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- XGBoost Classifier

### Development Environment
- Jupyter Notebook / Google Colab

---

# 🔍 Project Workflow

```
Data Collection
       |
       ↓
Data Exploration & Visualization
       |
       ↓
Data Preprocessing
       |
       ↓
Handling Class Imbalance (SMOTE)
       |
       ↓
Model Training
       |
       ↓
Model Evaluation
       |
       ↓
Fraud Prediction
```

---

# 📊 Exploratory Data Analysis

Performed analysis includes:

- Dataset structure inspection
- Missing value analysis
- Fraud vs non-fraud transaction distribution
- Transaction amount analysis
- Correlation analysis
- Feature distribution visualization

---

# ⚙️ Data Preprocessing

Steps performed:

- Checked missing values
- Removed unnecessary features
- Scaled numerical features
- Split data into training and testing datasets
- Applied SMOTE to balance fraud and non-fraud classes

### Why SMOTE?

Credit card fraud datasets are usually highly imbalanced because fraudulent transactions represent only a small percentage of total transactions.

SMOTE generates synthetic samples for the minority class, improving model learning and fraud detection performance.

---

# 🤖 Machine Learning Models

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

# 📈 Model Evaluation

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

# 🚀 How to Run the Project

## Clone Repository

```bash
git clone https://github.com/<your-username>/credit-card-fraud-detection.git
```

Navigate into the project folder:

```bash
cd credit-card-fraud-detection
```

# 💡 Key Learnings

- Understanding real-world fraud detection challenges.
- Working with highly imbalanced datasets.
- Applying SMOTE for class balancing.
- Comparing multiple machine learning algorithms.
- Evaluating classification models using appropriate metrics.

---

# 🔮 Future Improvements

- Deploy the model using Flask/FastAPI.
- Create an interactive fraud monitoring dashboard.
- Implement real-time transaction prediction.
- Use deep learning approaches such as Neural Networks.
- Integrate cloud deployment using AWS.

---

# 👩‍💻 Author

**Sandhya Rani**

Master's in Computer Science  
Machine Learning | Python | Data Science 

New Jersey Institute of Technology (NJIT)

GitHub: https://github.com/<your-username>

LinkedIn: https://linkedin.com/in/<your-profile>


