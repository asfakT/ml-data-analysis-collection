# 📧 Spam Mail Detection using Logistic Regression

Classifies emails as **Spam or Ham (Not Spam)** using TF-IDF vectorization and Logistic Regression.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project3_Spam_mail/Logistic_Regression.ipynb)

---

## 📌 Overview

- **Dataset:** 5,572 emails (spam + ham)
- **Split:** 80% training (4,457) / 20% testing (1,115)
- **Text Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency)

---

## 🎯 Actual Results

| Dataset | Accuracy |
|---------|----------|
| Training Data | 96.77% |
| Test Data | **96.68%** |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy
- **Model:** Logistic Regression
- **Text Feature Extraction:** TfidfVectorizer
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Project3_Spam_mail/
├── Logistic_Regression.ipynb   # Main notebook
├── mail_data.csv               # Dataset
└── README.md
```

---

## 🔍 Key Steps

1. Load and clean email dataset
2. Label encoding (spam = 0, ham = 1)
3. 80/20 Train-Test Split
4. TF-IDF feature extraction
5. Logistic Regression model training
6. Accuracy evaluation on train and test data
7. Real-time prediction on new email input

---

## 📊 Dataset Info

| Category | Count |
|----------|-------|
| Ham (Not Spam) | ~4,825 |
| Spam | ~747 |
| **Total** | **5,572** |

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project3_Spam_mail
pip install pandas numpy scikit-learn
jupyter notebook Logistic_Regression.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
