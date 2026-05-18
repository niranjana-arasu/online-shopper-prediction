# online-shopper-prediction
# Predicting Online Shopper Purchase Intentions Using Machine Learning

## Project Overview

E-commerce businesses lose significant revenue when they cannot identify which website visitors are likely to make a purchase. Accurately predicting purchase intent allows businesses to target high-intent customers with personalised offers and improve conversion rates.

This project builds and compares multiple supervised machine learning classifiers to predict whether an online shopper will complete a purchase, based on their browsing behaviour and session data.

---

## Problem Statement

Can machine learning models accurately predict whether an online shopper will make a purchase, using clickstream and session behavioural data?

---

## Dataset

- **Source:** Publicly available dataset (UCI Machine Learning Repository / Kaggle)
- **Features include:** Number of pages visited, session duration, bounce rate, exit rate, special day indicator, visitor type, browser, and region
- **Target variable:** Purchase completed (binary: Yes / No)

---

## Methodology

1. **Exploratory Data Analysis (EDA)** — distribution analysis, class imbalance check, correlation analysis
2. **Data Preprocessing** — encoding categorical variables, feature scaling, train/test split (80/20)
3. **Model Training & Comparison** — three classifiers trained and evaluated:
   - Logistic Regression (baseline)
   - Decision Tree Classifier
   - Random Forest Classifier
4. **Evaluation Metrics** — Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## Results

| Model | Notes |
|---|---|
| Logistic Regression | Interpretable baseline model |
| Decision Tree | Evaluated with varying depth parameters |
| **Random Forest** | **Best performing model — highest accuracy and F1-score** |

Random Forest consistently outperformed the other classifiers, demonstrating the advantage of ensemble methods for behavioural classification tasks.

---

## Technologies Used

- **Language:** Python 3
- **Libraries:** pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

---

## Key Findings

- Bounce rate and exit rate were among the strongest negative predictors of purchase completion
- Visitors arriving on special days (e.g. close to a public holiday) showed different purchase patterns
- Random Forest provided the best balance of precision and recall — important for minimising both missed conversions and wasted marketing spend

---

## About

This project was completed as part of an MSc in Data Science (Distinction) at Coventry University, 2023–2024.

**Author:** Niranjana Thirunavukkarasu
**LinkedIn:** www.linkedin.com/in/niranjanathirunavukkarasu
