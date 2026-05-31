# 🏦 Loan Prediction using Support Vector Machine (SVM)

Predicts whether a loan application will be **approved or rejected** based on applicant details using Support Vector Machine (SVM).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project4_Loan_Prediction/SVM.ipynb)

---

## 📌 Overview

- **Dataset:** 614 loan applications, 13 features
- **After cleaning:** 480 rows (null values dropped)
- **Split:** 90% training (432) / 10% testing (48)
- **Stratified split** to maintain class balance

---

## 🎯 Actual Results

| Dataset | Accuracy |
|---------|----------|
| Training Data | 79.86% |
| Test Data | **83.33%** |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Seaborn
- **Model:** Support Vector Machine (SVM) — Linear Kernel
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Project4_Loan_Prediction/
├── SVM.ipynb          # Main notebook
├── loan_data.csv      # Dataset
└── README.md
```

---

## 📊 Dataset Features

| Feature | Description |
|---------|-------------|
| Gender | Male / Female |
| Married | Yes / No |
| Dependents | 0 / 1 / 2 / 3+ |
| Education | Graduate / Not Graduate |
| Self_Employed | Yes / No |
| ApplicantIncome | Applicant monthly income |
| CoapplicantIncome | Co-applicant monthly income |
| LoanAmount | Loan amount requested |
| Loan_Amount_Term | Term of loan in months |
| Credit_History | Credit history (1 = good) |
| Property_Area | Rural / Semiurban / Urban |

---

## 🔍 Key Steps

1. Load and explore dataset (614 rows, 13 features)
2. Handle missing values (drop null rows)
3. Label encoding for categorical features
4. Data visualization (Education & Marital Status vs Loan Status)
5. 90/10 Stratified Train-Test Split
6. SVM model training (linear kernel)
7. Accuracy evaluation on train and test data

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project4_Loan_Prediction
pip install pandas numpy scikit-learn seaborn
jupyter notebook SVM.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
