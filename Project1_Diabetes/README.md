# 🩺 Diabetes Prediction using Machine Learning

A machine learning project that predicts whether a patient has diabetes using the **Pima Indians Diabetes Dataset** with multiple ML algorithms.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project1_Diabetes/Project1_Diabetes.ipynb)

---

## 📌 Overview

This project applies multiple supervised ML algorithms to classify patients as diabetic or non-diabetic. The dataset contains medical predictor variables such as glucose concentration, BMI, age, insulin, and blood pressure.

- **Dataset:** 768 patients, 9 features
- **Split:** 70% training / 30% testing
- **Class Distribution:** 34.90% diabetic, 65.10% non-diabetic

---

## 🎯 Actual Results (Test Data)

| Model | Accuracy |
|-------|----------|
| Naive Bayes (GaussianNB) | 74.03% |
| Random Forest | 74.46% |
| Logistic Regression (C=0.7) | 74.89% |
| Logistic Regression CV (Cross-validated) | 70.56% |

> Best model: **Logistic Regression** with 74.89% accuracy on test data.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib
- **Environment:** Jupyter Notebook / Google Colab
- **Dataset:** Pima Indians Diabetes Dataset (NIDDK)

---

## 📁 Project Structure

```
Project1_Diabetes/
├── Project1_Diabetes.ipynb   # Main notebook
├── pima-data.csv             # Processed dataset
├── pima-data-orig.csv        # Original dataset
└── README.md
```

---

## 🔍 Key Steps

1. Exploratory Data Analysis (EDA)
2. Correlation Matrix Analysis
3. Handling missing/zero values using mean imputation
4. 70/30 Train-Test Split
5. Model Training: Naive Bayes, Random Forest, Logistic Regression
6. Hyperparameter tuning (C value) for Logistic Regression
7. Cross-validation using LogisticRegressionCV

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open in Colab** badge above — no setup needed.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project1_Diabetes
pip install pandas numpy scikit-learn matplotlib
jupyter notebook Project1_Diabetes.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
