# Glucose Level Prediction 🧠

This project predicts the risk of abnormal glucose levels using the **Framingham Heart Study** dataset. Multiple machine learning models were applied to identify individuals at higher risk and improve healthcare decision-making.

## 📌 Objective
To classify individuals with abnormal glucose levels using medical and lifestyle features, with a focus on optimizing **AUC**, **recall**, and **F1-score** for the positive class.

## ⚙️ Models Used
- Logistic Regression (manual + RFE)
- Decision Tree (tuned)
- Random Forest (with SMOTE, ADASYN)
- XGBoost (with SMOTE & Voting)
- CatBoost + Borderline-SMOTE
- LightGBM + SMOTE-ENN
- Stacking & Polynomial Features

## 🔍 Results
- Best AUC achieved: **~0.69**
- Resampling improved recall and F1 for minority class
- No model crossed 0.75 AUC due to feature limitations

## 🧠 What We Learned
- Key features: BMI, age, blood pressure
- Advanced resampling helps but cannot fully solve weak class separability
- Predictive modeling can support early intervention in preventive care


---

## ✅ Run the Project
```bash
pip install -r requirements.txt
