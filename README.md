# 🫀 Heart Disease – Exploratory Data Analysis

Comprehensive **Exploratory Data Analysis (EDA)** and baseline modeling on the Heart Disease dataset.  
The goal is to analyze clinical and exercise-test features that are most associated with heart disease.

---

## 📘 1. Project Overview

This project explores how patient attributes (age, cholesterol, ECG results, etc.) correlate with the target label **HeartDisease**.

Key objectives:
- Clean and preprocess raw heart dataset  
- Perform statistical and visual EDA  
- Identify top predictive signals  
- Train baseline models (Logistic Regression and Random Forest)

---

## 🧩 2. Dataset Description

**Target column**
- `HeartDisease`: `1` → presence of heart disease, `0` → no disease.

**Feature summary**

| Feature | Type | Meaning |
|----------|------|----------|
| `Age` | Numeric | Age in years |
| `Sex` | Categorical | M/F |
| `ChestPainType` | Categorical | TA, ATA, NAP, ASY |
| `RestingBP` | Numeric | Resting systolic BP (mmHg) |
| `Cholesterol` | Numeric | Serum cholesterol (mg/dL) |
| `FastingBS` | Binary | 1 if Fasting Blood Sugar >120 mg/dL |
| `RestingECG` | Categorical | Normal, ST, LVH |
| `MaxHR` | Numeric | Max heart rate during exercise (bpm) |
| `ExerciseAngina` | Binary | Y if exercise-induced angina |
| `Oldpeak` | Numeric | ST-segment depression relative to rest |
| `ST_Slope` | Ordinal | Up, Flat, Down (slope of ST segment) |

### Medical meaning of key terms
- **ECG (Electrocardiogram)**: records electrical activity of the heart.  
- **ST Segment**: flat portion between QRS and T-wave; depression (Oldpeak) indicates ischemia.  
- **Oldpeak**: numeric measure of that depression in mm.  
- **ST_Slope**: shape of the ST segment during stress — a strong indicator of disease.

---

## ⚙️ 3. Setup Instructions

### Requirements
Python ≥ 3.8  
Install dependencies:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn scipy
