# 🚗 Car Price Prediction using Linear Regression

Predicts used car selling prices using **Linear Regression** and **Lasso Regression** based on features like fuel type, transmission, year, and kilometers driven.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Project2_Car_prize_prediction/LinearRegression.ipynb)

---

## 📌 Overview

- **Dataset:** 301 used cars with features like year, present price, kms driven, fuel type, seller type, and transmission
- **Target:** Selling Price
- **Split:** 90% training / 10% testing

---

## 🎯 Actual Results

| Dataset | R² Score |
|---------|----------|
| Training Data | 0.8799 (87.99%) |
| Test Data | 0.8366 (83.66%) |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, Matplotlib, Seaborn
- **Models:** Linear Regression, Lasso Regression
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Project2_Car_prize_prediction/
├── LinearRegression.ipynb   # Main notebook
├── car data.csv             # Dataset
└── README.md
```

---

## 🔍 Key Steps

1. Exploratory Data Analysis (EDA)
2. Categorical Encoding (Fuel Type, Seller Type, Transmission)
3. 90/10 Train-Test Split
4. Linear Regression model training
5. R² Score evaluation on train and test data
6. Actual vs Predicted price visualization

---

## 📊 Dataset Features

| Feature | Description |
|---------|-------------|
| Year | Manufacturing year |
| Present_Price | Current ex-showroom price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Petrol / Diesel / CNG |
| Seller_Type | Dealer / Individual |
| Transmission | Manual / Automatic |
| Owner | Number of previous owners |

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the **Open In Colab** badge above.

### Option 2: Local
```bash
git clone https://github.com/asfakT/ml-data-analysis-collection.git
cd ml-data-analysis-collection/Project2_Car_prize_prediction
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook LinearRegression.ipynb
```

---

## 👨‍💻 Author

**Asfak Shahrier**
- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
