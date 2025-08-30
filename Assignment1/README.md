# Machine Learning Lab Experiments

This repository contains multiple machine learning experiments implemented in Python.  
It was originally created as part of coursework.

## 📌 Experiments

### 1. IRIS Dataset - Logistic Regression
- Loads the **Iris dataset** using seaborn.
- Performs feature selection using `SelectKBest`.
- Splits the dataset and trains a Logistic Regression model.
- Evaluates performance using a confusion matrix and classification report.

### 2. Loan Amount Prediction - Linear Regression
- Generates a dummy **loan dataset** and saves it as `train.csv`.
- Preprocesses the dataset (dropping irrelevant columns, handling categorical variables).
- Trains a Linear Regression model to predict loan sanction amount.
- Evaluates performance using RMSE and R² Score.
- Plots **Actual vs Predicted Loan Amounts**.

### 3. Diabetes Dataset - Random Forest Classifier
- Loads the **diabetes.csv** dataset (must be placed in Google Drive).
- Trains a Random Forest classifier to predict diabetes outcome.
- Evaluates with accuracy, confusion matrix, classification report, feature importance, and ROC curve.

### 4. Spam Dataset - Naive Bayes
- Loads the **Spambase dataset** from UCI ML Repository (`spambase.data`).
- Trains a Gaussian Naive Bayes classifier.
- Evaluates accuracy and classification report.
- Visualizes spam vs non-spam distribution.

### 5. MNIST Digits Dataset - Logistic Regression
- Loads the **MNIST Digits dataset** from sklearn.
- Trains Logistic Regression for digit classification.
- Evaluates accuracy and generates a classification report.

---

## ⚙️ Requirements

Install the required Python packages before running the experiments:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## ▶️ How to Run

Run the script:

```bash
python mllaba1.py
```

Ensure that:
- `diabetes.csv` is available in the correct path.
- `spambase.data` is available in the correct path.

---

## 📂 Files
- **mllaba1.py** → Main Python script containing all experiments
- **train.csv** → Auto-generated dummy loan dataset
- **diabetes.csv** → Required dataset (must be provided)
- **spambase.data** → Required dataset (must be provided)

---

## 👤 Author
**Sudharshan Vijayaragavan**  
Reg No: 3122237001054
