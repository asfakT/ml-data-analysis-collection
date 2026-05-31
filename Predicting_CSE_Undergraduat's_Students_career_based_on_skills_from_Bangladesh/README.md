# 🎓 Predicting CSE Undergraduate Students' Careers Using Machine Learning

A **multi-label career prediction** research project for CSE undergraduates in Bangladesh using real survey data from 468 students across 47 universities.

> 📄 **Research Paper:** "Predicting CSE Undergraduate Students' Careers Using Machine Learning Algorithms in the Context of Bangladesh" — Under Review

| Notebook | Description | Link |
|----------|-------------|------|
| 📦 Preprocessing | Data cleaning, encoding, normalization | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Predicting_CSE_Undergraduat's_Students_career_based_on_skills_from_Bangladesh/Preprocessing.ipynb) |
| 📊 Data Analysis | EDA, visualizations, correlation heatmap | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Predicting_CSE_Undergraduat's_Students_career_based_on_skills_from_Bangladesh/r2_data_analysis.ipynb) |
| 🤖 ML Models | Model training, evaluation, comparison | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/asfakT/ml-data-analysis-collection/blob/main/Predicting_CSE_Undergraduat's_Students_career_based_on_skills_from_Bangladesh/r2_ML_part.ipynb) |

---

## 📌 Overview

This is the **first multi-label career prediction framework** for Bangladeshi CSE undergraduates using real institutional data. Unlike prior studies that predict only one career outcome, this model recommends **multiple relevant career sectors** based on a student's skills, academic performance, and preferences.

- **Dataset:** 468 CSE students from 47 public and private universities in Bangladesh
- **Features:** 24 attributes (CGPA, soft skills, technical skills, research skills, publications, projects, influencing factors, preferred job sectors)
- **Survey Period:** April 24, 2024 – November 21, 2024
- **Task:** Multi-label classification (10 career categories)
- **Train-Test Split:** 80% / 20%

---

## 🎯 Actual Results — All 10 Models Compared

| Model | Accuracy (%) | Precision | Recall | F1 Micro | F1 Macro | Hamming Loss | Time (s) |
|-------|-------------|-----------|--------|----------|----------|--------------|----------|
| **XGBoost** | **61.70** | **0.856** | **0.737** | **0.792** | **0.695** | **0.060** | 0.75 |
| KNN | 55.31 | 0.876 | 0.634 | 0.736 | 0.538 | 0.070 | 0.09 |
| Hard Voting | 51.06 | 0.852 | 0.650 | 0.767 | 0.651 | 0.062 | 1.80 |
| Soft Voting | 51.06 | 0.861 | 0.665 | 0.761 | 0.651 | 0.063 | 1.79 |
| Gradient Boosting | 51.06 | 0.888 | 0.648 | 0.749 | 0.589 | 0.067 | 1.71 |
| Random Forest | 47.87 | 0.910 | 0.620 | 0.737 | 0.517 | 0.061 | 1.57 |
| Neural Network | 47.87 | 0.799 | 0.627 | 0.697 | 0.579 | 0.080 | 3.47 |
| SVM | 43.61 | 0.716 | 0.577 | 0.677 | 0.531 | 0.082 | 0.37 |
| Logistic Regression | 42.55 | 0.811 | 0.625 | 0.703 | 0.551 | 0.081 | 0.09 |
| Decision Tree | 37.23 | 0.671 | 0.689 | 0.680 | 0.525 | 0.100 | 0.08 |

> **Best Model: XGBoost** — highest accuracy (61.70%), best Recall, best F1 Micro, best F1 Macro, lowest Hamming Loss.
>
> Note: Lower accuracy compared to single-label tasks is expected in multi-label classification where students can belong to multiple career categories simultaneously.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy, Matplotlib, Seaborn
- **Models:** Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, XGBoost, Hard Voting, Soft Voting, SVM, Neural Network (MLP), KNN
- **Encoding:** MultiLabelBinarizer (multi-hot vectors), OrdinalEncoder
- **Normalization:** StandardScaler
- **Environment:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
Predicting_CSE_Undergraduat's_Students_career_based_on_skills_from_Bangladesh/
├── Preprocessing.ipynb       # Data cleaning, encoding, normalization
├── r2_data_analysis.ipynb    # EDA, visualizations, correlation heatmap
├── r2_ML_part.ipynb          # Model training, evaluation, comparison
├── dataset.csv               # Survey data (468 students, 24 features)
└── README.md
```

---

## 📊 Dataset Features (24 Attributes)

| Category | Features |
|----------|---------|
| Personal Info | Gender, Year, CGPA |
| Soft Skills | Critical Thinking, Problem Solving, Teamwork, Communication |
| Technical Skills | Software Engineering, DSA, Database, Data Analysis, Web Dev, Computer Architecture, OS, Networking, Cyber Security, ML, Robotics |
| Research | Research Skill, Publications, Projects |
| Influencing Factors | Social Acceptance, Job Security, Salary, Job Environment, Work-Life Balance |
| Target (18 job roles) | Software Development, ML/AI, Data Analysis, Cyber Security, Networking, Teaching, Researcher, Abroad, Govt Job, BCS, Bank Job, and more |

---

## 🔍 Key Steps

### 📦 Notebook 1: Preprocessing
1. Load raw survey data (468 responses)
2. Handle missing values (zero/unrated imputation)
3. Ordinal encoding for skill ratings (0=Unrated, 1=Basic, 2=Intermediate, 3=Advanced)
4. MultiLabelBinarizer for multi-hot target vectors
5. Feature reduction (remove timestamp, email, irrelevant fields)
6. StandardScaler normalization

### 📊 Notebook 2: Data Analysis
1. Career preference distribution (Software Dev = 48.7% most preferred)
2. CGPA and soft skill distribution analysis
3. Technical skill distribution across students
4. Project vs Publication comparison (boxplot)
5. Influencing factors per career category
6. Correlation heatmap (24 features)
7. Association rule mining (Bank Job + BCS + Govt Job co-occurrence)

### 🤖 Notebook 3: ML Models
1. 80/20 Train-Test Split
2. Train 10 ML classifiers with hyperparameter tuning
3. Evaluate: Accuracy, Precision, Recall, F1 Micro, F1 Macro, Hamming Loss
4. Test sample evaluation (2 student profiles)
5. Model comparison visualization

---

## 📈 Key Findings

- **Software Development** is the most preferred career (48.7% of students)
- **XGBoost** outperforms all models across all multi-label metrics
- **CGPA + Research Skills + Project Count** are the top predictors
- Students with strong research profiles → predicted for **Abroad / Researcher**
- Students with strong applied skills → predicted for **Software Sector**
- **Salary** is the main influencing factor for technical careers

---

## 🔗 Dataset & Code

- 📊 Dataset: [GitHub CSV](https://github.com/IsratJahanR/CSE-Thesis/blob/main/CSE%20Thesis%20-%20Sheet1.csv)
- 💻 Original Code Repository: [IsratJahanR/CSE-Thesis](https://github.com/IsratJahanR/CSE-Thesis)

---

## 👨‍💻 Authors

**Asfak Shahrier** & Israt Jahan Reshma
Department of Computer Science and Engineering
Gopalganj Science and Technology University, Bangladesh

- Portfolio: [asfakshahrier.com](https://asfakshahrier.com)
- GitHub: [@asfakT](https://github.com/asfakT)
- LinkedIn: [linkedin.com/in/asfak-shahrier](https://linkedin.com/in/asfak-shahrier)
- Email: shahrierasfak27@gmail.com
