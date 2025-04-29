<p align="center">
  <strong>Predicting customer subscription to term deposits using a structured two-phase machine learning workflow, including pre-call and post-call modeling, feature engineering, and customer segment profiling.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Project-Term_Deposit_Subscription_Prediction-blueviolet?style=for-the-badge" alt="Project Badge">
</p>

# Term Deposit Subscription Prediction Project

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?style=flat-square">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Machine_Learning-Yes-lightgrey?style=flat-square">
  <img src="https://img.shields.io/badge/Framework-Scikit--Learn-orange?style=flat-square">
</p>


[View the project notebook here](https://github.com/AlvinSMoyo/8Pl5KRkI1SP3AL13)

---

## 📚 Project Overview

This project was completed during my AI Residency at [Apziva](https://www.apziva.com/), focusing on predicting customer subscription to term deposit products based on customer demographics and call metadata.  
The goal was to develop a two-phase predictive modeling strategy to optimize marketing efficiency and improve subscription rates.

---
## 📚 Dataset

- **Source**: The dataset used is "term-deposit-marketing-2020," reflecting a real-world business problem.  
- **Context**: It originates from direct marketing campaigns conducted by a European banking institution.  
- **Features**: Include customer demographics (age, job, marital status) and call campaign metadata (contact type, call duration, frequency of contact).


---
## 🚀 Project Workflow

The project was executed in a structured, phased approach:

### 1. 📊 Exploratory Data Analysis (EDA)
- Conducted deep statistical analysis, distribution checks, and feature correlations.
- Identified key patterns affecting subscription likelihood.

### 2. 🛠️ Feature Engineering
- Created new features like `contact_frequency` and `call_duration_category`.
- Handled outliers and encoded categorical variables.

### 3. 🧪 Pre-Call Modeling (Before Contacting Customers)
- Objective: Predict customers unlikely to subscribe before making contact.
- Balanced imbalanced classes using ADASYN.
- Trained models including Complement Naive Bayes (final selected model).
- Prioritized **high precision** to reduce unnecessary outreach.

### 4. 📞 Post-Call Modeling (After Customer Interaction)
- Objective: Predict customers likely to subscribe after calls.
- Focused on models like XGBoost (final selected model after tuning).
- Evaluated using Precision-Recall curves and threshold tuning.

### 5. 🔍 Clustering & Segment Profiling
- Conducted hierarchical clustering on customer segments.
- Visualized segments using PCA, t-SNE, and UMAP.
- Identified high-conversion customer profiles for marketing targeting.

### 6. 🚀 DuckDB Optimization (Bonus)
- Integrated DuckDB to accelerate data querying and feature extraction for larger datasets.

---
## 🎯 Key Outcomes

| Phase | Best Model | Key Metric | Strategic Impact |
|:------|:-----------|:-----------|:-----------------|
| Pre-Call | Complement Naive Bayes (threshold=0.48) | 59% Recall | Early filtering of unlikely subscribers |
| Post-Call | XGBoost Classifier (threshold tuned) | 74.9% F1 Score | Prioritized calling high-likelihood subscribers |

---

## 📈 Visual Highlights

- ROC and Precision-Recall curve comparisons to show model trade-offs.
- Confusion matrix heatmaps to embellish contrast between predicted and actual values.
- Cluster visualizations demonstrating separable customer segments.
- Segment success rate analysis to guide marketing resource allocation.

---

## 🙏 Thank You for Reading!

This project was completed by **Alvin Siphosenkosi Moyo** as part of my AI Residency at Apziva.  
Feel free to connect with me:

- [LinkedIn Profile](https://www.linkedin.com/in/alvin-moyo-5a711021)
- [GitHub Portfolio](https://github.com/AlvinSMoyo)

---

## 💼 Concluding Remarks

This project demonstrates a strong end-to-end applied machine learning workflow, covering:

- Data preprocessing, feature engineering, and class balancing strategies
- Model benchmarking, hyperparameter tuning, and threshold optimization
- Business-driven modeling objectives aligned with real-world marketing goals
- Clear communication of technical results through visualizations and strategic insights

This work highlights my ability to design and deliver practical machine learning solutions with technical depth, business understanding, and clarity of presentation.

Thank you for taking the time to review this project!

---

# 🚀 Thank you for reviewing my work!
