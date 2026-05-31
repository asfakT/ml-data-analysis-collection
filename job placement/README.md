# 💼 Job Placement Prediction using Logistic Regression

Predicts whether a student will get **placed or not** based on CGPA and IQ score using Logistic Regression with decision boundary visualization.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/job%20placement/job%20placement.ipynb)

---

## 📌 Overview

- **Dataset:** 100 students with CGPA and IQ scores
- **Target:** Placement (1 = Placed, 0 = Not Placed)
- **Split:** 90% training (90) / 10% testing (10)
- **Features:** CGPA, IQ Score only

---

## 🎯 Actual Results

| Dataset | Accuracy |
|---------|----------|
| Test Data | **80%** |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, mlxtend
- **Model:** Logistic Regression
- **Visualization:** Decision Region Plot (mlxtend)
- **Deployment:** Model saved with Pickle
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
job placement/
├── job placement.ipynb   # Main notebook
├── placement.csv         # Dataset (100 students)
├── model.pkl             # Saved Logistic Regression model
└── README.md
```

---

## 🔍 Key Steps

1. Load dataset (100 students, CGPA + IQ + Placement)
2. Feature selection (drop index column)
3. Scatter plot visualization (CGPA vs IQ colored by placement)
4. 90/10 Train-Test Split
5. StandardScaler normalization
6. Logistic Regression model training
7. Accuracy evaluation (80% on test data)
8. Decision boundary visualization using mlxtend
9. Model saved with Pickle for deployment

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd "ml-data-analysis-collection/job placement"
pip install pandas numpy scikit-learn matplotlib mlxtend
jupyter notebook "job placement.ipynb"
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
