# Titanic-Dataset
# 🚢 Titanic Survival Prediction

A machine learning project to predict whether a passenger survived the Titanic disaster using classification algorithms.

---

## 📌 Problem Statement

The sinking of the Titanic on April 15, 1912 led to the death of 1502 out of 2224 passengers and crew. This project builds a predictive model to answer:

> **"What kinds of people were more likely to survive?"**

Using passenger features like age, gender, ticket class, and fare to predict survival (1 = Alive, 0 = Dead).

---

## 📂 Dataset

- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- **Total Records:** ~891 rows (training set)
- **Target Variable:** `Survived` (1 = Alive, 0 = Dead)
- **Class Distribution:** ~67.5% Dead · ~32.5% Alive

| Feature | Description |
|---|---|
| Pclass | Ticket class (1st, 2nd, 3rd) |
| Sex | Gender of passenger |
| Age | Age in years |
| SibSp | No. of siblings/spouses aboard |
| Parch | No. of parents/children aboard |
| Fare | Passenger fare |
| Embarked | Port of embarkation |

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn

---

## ⚙️ Project Workflow

1. **Data Loading** — Load and explore the Titanic dataset
2. **EDA** — Understand survival patterns across gender, class, age
3. **Data Cleaning** — Handle missing values (Age, Embarked, Cabin)
4. **Feature Engineering** — Encode categorical variables
5. **Model Building** — Train Logistic Regression classifier
6. **Evaluation** — Confusion matrix, accuracy, precision, recall, F1, ROC curve

---

## 📊 Model Performance (Logistic Regression)

| Metric | Score |
|---|---|
| Accuracy | **0.8065** |
| Precision | 0.7547 |
| Recall | 0.7018 |
| F1 Score | 0.7273 |
| AUC-ROC | ~0.85 |

### Confusion Matrix

```
              Predicted
              Alive   Dead
Actual Alive  [ 85     13 ]
Actual Dead   [ 17     40 ]
```

- **True Positives (TP):** 85 — correctly predicted survivors
- **True Negatives (TN):** 40 — correctly predicted deaths
- **False Positives (FP):** 13 — predicted alive, actually dead
- **False Negatives (FN):** 17 — predicted dead, actually alive ⚠️

---

