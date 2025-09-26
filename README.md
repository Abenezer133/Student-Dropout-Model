# 🎓 Student Dropout Risk Prediction

This is my first applied machine learning project.  
The idea was to see if simple student data can be used to predict who might be at risk of dropping out.  
I wanted to learn not only about models, but also about how to explain them.

---

## 📌 Project Overview

- **Problem:** Many schools only notice dropout risk when it’s already too late.  
- **Goal:** Build a small prototype model to flag students earlier.  
- **Approach:**  
  - Tried Logistic Regression (baseline)  
  - Tried XGBoost (more powerful)  
  - Used SHAP for interpretability (to see which features matter)  
  - Measured performance with F1-score and Precision@Top10%  

---

## ⚙️ Features Used

- `attendance_rate` → percentage of classes attended  
- `avg_grade` → average grade across assignments/exams  
- `late_submissions` → number of late assignments  
- `lms_activity` → engagement on the learning platform  

---

## 📊 Results

- **Logistic Regression (baseline):** F1 = **0.50**  
- **XGBoost (best):** F1 = **1.0** (on this small dataset — probably overfitting)  
- **Precision@Top10%:** 1.0 → the top 10% most “at-risk” students flagged by the model were truly at risk  
- **SHAP explainability:** attendance rate and average grade were the most important factors  

*(Since the dataset was small and simulated, the XGBoost results look “too perfect.” In real life with bigger data, results would be more realistic.)*  

🧠 **What I Learned**

How to build and compare ML models (baseline vs advanced)

The importance of explainability in sensitive applications like education

Why overfitting happens and how to watch out for it

How to evaluate model performance beyond accuracy (e.g. F1, precision@top%)
---

## 🚀 How to Run

1. Open the notebook in **Google Colab** (this repo includes a link).  
2. Install dependencies:  
