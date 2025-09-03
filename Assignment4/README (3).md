# Ensemble Prediction and Decision Tree Model Evaluation

## 📌 Course Information
- **Institution:** Sri Sivasubramaniya Nadar College of Engineering, Chennai  
- **Degree & Branch:** M.Tech (Integrated) Computer Science & Engineering (Batch 2023–2028)  
- **Semester:** V  
- **Subject Code & Name:** ICS1512 – Machine Learning Algorithms Laboratory  
- **Academic Year:** 2025–2026 (Odd Semester)  
- **Experiment No.:** 3  

---

## 🎯 Objective
To build classifiers such as **Decision Tree, AdaBoost, Gradient Boosting, XGBoost, Random Forest, and Stacking Models** and evaluate their performance through **5-Fold Cross-Validation** and **hyperparameter tuning**.

---

## 📊 Dataset
- **Name:** Wisconsin Diagnostic Breast Cancer (WDBC) Dataset  
- **Samples:** 569  
- **Features:** 30 numerical attributes describing cell nuclei characteristics  
- **Target:** Binary (Malignant = 1, Benign = 0)  
- **Source:** [UCI Repository](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)

---

## ⚙️ Steps for Implementation
1. Load and preprocess dataset  
   - Encode labels  
   - Handle missing values  
   - Standardize features  

2. Perform Exploratory Data Analysis (EDA)  
   - Class distribution  
   - Feature correlation  

3. Split dataset into Train, Validation, and Test sets (70/15/15).  

4. Train models:
   - Decision Tree  
   - AdaBoost  
   - Gradient Boosting  
   - XGBoost  
   - Random Forest  
   - Stacking/Voting Classifier (Decision Tree + Random Forest, etc.)  

5. Tune hyperparameters using **GridSearchCV** with **5-Fold Stratified Cross-Validation**.  

6. Record best hyperparameters and evaluate performance.  

7. Compute metrics: Accuracy, Precision, Recall, F1-Score.  

8. Plot **ROC curves** and compare AUC for all models.  

---

## 📚 Libraries Used
- `pandas`, `numpy`  
- `matplotlib`, `seaborn`  
- `scikit-learn` (`DecisionTreeClassifier`, `AdaBoostClassifier`, `GradientBoostingClassifier`, `RandomForestClassifier`, `VotingClassifier`)  
- `xgboost`  
- `Google Colab` (for execution environment & Drive mount)  

---

## 📈 Results & Evaluation
- Each model was optimized via **GridSearchCV** with cross-validation.  
- Evaluation was done on a held-out **test set**.  
- Metrics included **Accuracy, Precision, Recall, F1-score, and AUC**.  
- ROC curves were plotted for model comparison.  

---

## 📌 Observations
- Ensemble methods (AdaBoost, Gradient Boosting, XGBoost, Random Forest) generally outperformed the standalone Decision Tree.  
- Random Forest benefited from hyperparameter tuning (e.g., `max_depth`, `n_estimators`).  
- Stacking/Voting models improved generalization compared to single classifiers.  
- The best model achieved high accuracy and robustness with minimal overfitting.  

---

## ✅ How to Run
1. Clone the repo or download the `.py` file.  
2. Ensure dependencies are installed:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost
   ```
3. Run the script in Python or Jupyter/Colab:  
   ```bash
   python ml_assgn4.py
   ```
4. View printed evaluation metrics and ROC curve plots.  

---

## 📖 References
- [Scikit-learn: Decision Trees](https://scikit-learn.org/stable/modules/tree.html)  
- [Scikit-learn: Ensemble Methods](https://scikit-learn.org/stable/modules/ensemble.html)  
- [XGBoost Documentation](https://xgboost.readthedocs.io/en/latest/)  
- [UCI Breast Cancer Dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)  
