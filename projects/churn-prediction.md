---
layout: default
title: Customer Churn Prediction
---

# Customer Churn Prediction

**Problem.** Reduce subscription churn for a B2C SaaS by predicting which users are most at risk.

**Data.** 65K users, 120 features (usage events, tenure, support tickets).

**Approach.**
- Cleaned & joined sources (SQL + Pandas), feature engineered recency/frequency, rolling aggregates.
- Trained **XGBoost** and **Logistic Regression** baselines with nested cross-validation.
- Used **SHAP** for global and local explainability; built a cost-sensitive decision rule.

**Results.**
- AUC = **0.87**, top decile capture = **41%**, estimated **−18% churn** in pilot group.
- Deployed a weekly scoring job and a lightweight **Streamlit** app for CX teams.

**Links.**
- Code: <https://github.com/YOUR_GH/churn-model>
- App: <https://your-streamlit-app.example.com>
- Back to [Home](/)