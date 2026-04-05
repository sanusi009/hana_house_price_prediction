# hana_house_price_prediction
# 🏠 House Price Prediction with SAP HANA & Python

![Python](https://img.shields.io/badge/Python-3.12-blue)
![SAP HANA](https://img.shields.io/badge/SAP%20HANA-Cloud-orange)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A complete end-to-end Machine Learning pipeline using **SAP HANA Cloud** as the data backend and **Python** for model training and visualization.

---

## 📌 Project Overview

This project predicts California house prices using three ML models, with data stored and managed in SAP HANA Cloud.

### Pipeline
```
SAP HANA Cloud (Data Storage)
        │
        ▼
Exploratory Data Analysis (EDA)
        │
        ▼
Feature Engineering & Train/Test Split
        │
        ▼
Model Training
  ├── Linear Regression  (Baseline)
  ├── Random Forest      (Ensemble)
  └── Gradient Boosting  (Best Model)
        │
        ▼
Model Comparison & Evaluation
        │
        ▼
Save Predictions → SAP HANA Cloud
```

---

## 📊 Results

| Model | RMSE | MAE | R² Score |
|---|---|---|---|
| Linear Regression | ~0.73 | ~0.53 | ~0.60 |
| Random Forest | ~0.52 | ~0.36 | ~0.82 |
| **Gradient Boosting** | **~0.47** | **~0.32** | **~0.85** |

---

## 🛠️ Tech Stack

- **Database:** SAP HANA Cloud (Free Tier)
- **Language:** Python 3.12
- **Libraries:** `hana_ml`, `hdbcli`, `scikit-learn`, `pandas`, `matplotlib`, `seaborn`
- **Environment:** Google Colab

---



## 📁 Project Structure

```
hana-house-price-prediction/
│
├── 📓 hana_house_price_prediction.ipynb   # Main notebook
├── 📋 README.md                           # This file
├── 📦 requirements.txt                    # Dependencies
└── 🖼️  screenshots/                       # Output plots
    ├── eda_plots.png
    ├── model_comparison.png
    └── feature_importance.png
```

---

## 📈 Key Findings

- **Income (MedInc)** is the strongest predictor of house prices (~59% importance)
- **Location (Lat/Long)** accounts for ~21% of predictions
- **Gradient Boosting** outperforms other models with R²=0.845

---

## 📝 License
MIT License — feel free to use and modify!
