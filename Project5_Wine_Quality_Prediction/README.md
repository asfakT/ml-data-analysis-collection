# 🍷 Wine Quality Prediction using Random Forest

Predicts whether a red wine is **Good Quality or Bad Quality** based on physicochemical properties using Random Forest Classifier.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project5_Wine_Quality_Prediction/wine_quality_prediction.ipynb)

---

## 📌 Overview

- **Dataset:** 1,599 red wine samples, 12 features
- **Target:** Quality score → Binary (Good = 1 if quality ≥ 7, Bad = 0)
- **Split:** 80% training (1,279) / 20% testing (320)
- **No missing values** in dataset

---

## 🎯 Actual Results

| Dataset | Accuracy |
|---------|----------|
| Test Data | **92.81%** |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **Model:** Random Forest Classifier
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Project5_Wine_Quality_Prediction/
├── wine_quality_prediction.ipynb   # Main notebook
├── winequality-red.csv             # Dataset
└── README.md
```

---

## 📊 Dataset Features

| Feature | Description |
|---------|-------------|
| fixed acidity | Tartaric acid content |
| volatile acidity | Acetic acid content |
| citric acid | Citric acid content |
| residual sugar | Sugar remaining after fermentation |
| chlorides | Salt content |
| free sulfur dioxide | Free SO₂ |
| total sulfur dioxide | Total SO₂ |
| density | Wine density |
| pH | Acidity level |
| sulphates | Sulphate content |
| alcohol | Alcohol percentage |
| quality | Score (0–10) → binarized to Good/Bad |

---

## 🔍 Key Steps

1. Load dataset (1,599 samples, no missing values)
2. Data visualization (quality distribution, correlation heatmap)
3. Label binarization (quality ≥ 7 = Good, else Bad)
4. 80/20 Train-Test Split
5. Random Forest Classifier training
6. Accuracy evaluation on test data
7. Real-time prediction on new wine sample

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project5_Wine_Quality_Prediction
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook wine_quality_prediction.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
