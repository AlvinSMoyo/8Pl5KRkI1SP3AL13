# Term Deposit Subscription Prediction Project

[View the project notebook here](https://github.com/AlvinSMoyo/8Pl5KRkI1SP3AL13)

---

## 📌 Project Overview

This project was completed during my AI Residency at Apziva, focusing on predicting customer subscription to term deposit products based on customer demographics and call metadata.  
The goal was to develop a two-phase predictive modeling strategy to optimize marketing efficiency and improve subscription rates.

---
## 📚 Dataset

- Source: [Custom project dataset provided via Google Drive](https://drive.google.com/file/d/1EW-XMnGfxn-qzGtGPa3v_C63Yqj2aGf7)
- Description: This dataset is based on the Term Deposit Marketing concept, adapted and enhanced for educational and applied machine learning purposes.
- Features include customer demographics (age, job, marital status) and call campaign metadata (contact type, call duration, frequency of contact).

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

- Clear ROC and Precision-Recall curves to show model trade-offs.
- Cluster visualizations demonstrating separable customer segments.
- Segment success rate analysis to guide marketing resource allocation.

---

## 👨‍💻 About the Author

This project was completed by **Alvin Siphosenkosi Moyo** as part of my AI Residency at Apziva.  
Feel free to connect with me:

- [LinkedIn Profile](https://www.linkedin.com/in/alvin-moyo-5a711021)
- [GitHub Portfolio](https://github.com/AlvinSMoyo)

---

## 💼 Concluding Remarks

This project showcases end-to-end applied machine learning expertise, including:

- Data preprocessing, feature engineering, and balancing strategies
- Model benchmarking, hyperparameter tuning, and threshold optimization
- Business-driven modeling objectives aligned with marketing goals
- Clear communication of technical results through clean visualizations and business insights

**Hiring managers and recruiters:**  
This project highlights my ability to build real-world, business-impactful machine learning solutions with professionalism, technical depth, and clarity.  
I am open to global remote opportunities or Saudi-based roles in Data Science, AI, and Advanced Analytics.

---

# 🚀 Thank you for reviewing my work!
