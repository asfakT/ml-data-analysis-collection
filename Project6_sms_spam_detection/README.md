# 📱 SMS Spam Detection using NLP & Machine Learning

Classifies SMS messages as **Spam or Ham** using NLP text preprocessing and multiple ML algorithms with TF-IDF vectorization.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project6_sms_spam_detection/sms_spam_detection.ipynb)

---

## 📌 Overview

- **Dataset:** 5,572 SMS messages → 5,169 after removing 403 duplicates
- **Class Distribution:** 4,516 Ham (87.2%) / 653 Spam (12.8%)
- **Split:** 80% training / 20% testing
- **Text Vectorization:** TF-IDF (max 3,000 features)

---

## 🎯 Actual Results — All Models Compared

| Model | Accuracy | Precision |
|-------|----------|-----------|
| BernoulliNB | 98.36% | 99.19% |
| Voting Classifier (SVM+NB+ETC) | **98.16%** | **99.17%** |
| SVC | 97.58% | 97.48% |
| Random Forest | 97.58% | 98.29% |
| Extra Trees | 97.49% | 97.46% |
| MultinomialNB | 97.10% | 100% |
| Logistic Regression | 95.84% | 97.03% |
| XGBoost | 96.71% | 92.62% |
| AdaBoost | 96.03% | 92.92% |
| Decision Tree | 93.33% | 84.16% |
| KNN | 90.52% | 100% |

> Best model: **BernoulliNB** (98.36% accuracy, 99.19% precision)

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, NLTK, Pandas, NumPy, Matplotlib, Seaborn, WordCloud, XGBoost
- **Text Processing:** TF-IDF, Tokenization, Stemming, Stopword Removal
- **Models:** Naive Bayes, SVM, Random Forest, XGBoost, Voting Classifier, and more
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Project6_sms_spam_detection/
├── sms_spam_detection.ipynb   # Main notebook
├── spam.csv                   # Dataset
├── vectorizer.pkl             # Saved TF-IDF vectorizer
├── model.pkl                  # Saved MultinomialNB model
└── README.md
```

---

## 🔍 Key Steps

1. Data cleaning (drop duplicates, rename columns)
2. Label encoding (spam = 1, ham = 0)
3. EDA — class distribution, word clouds, character/word stats
4. NLP preprocessing — lowercase, tokenize, remove stopwords, stemming (PorterStemmer)
5. TF-IDF vectorization (3,000 features)
6. Train and compare 11 ML models
7. Voting Classifier (SVM + NB + ExtraTrees) ensemble
8. Save model with pickle for deployment

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project6_sms_spam_detection
pip install pandas numpy scikit-learn nltk matplotlib seaborn wordcloud xgboost
jupyter notebook sms_spam_detection.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
