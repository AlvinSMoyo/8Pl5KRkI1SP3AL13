# 📊 Term Deposit Subscription Prediction (Apziva Project)

**Author**: Alvin Siphosenkosi Moyo  
**Status**: Completed (2025)  
**Domain**: Banking & Marketing Analytics  
**Tools**: Python, Pandas, Scikit-learn, XGBoost, SMOTE, Matplotlib, Seaborn  

---

## 🧠 Project Objective

The primary goal of this project was to **predict whether a bank customer would subscribe to a term deposit** based on historical marketing campaign data. This was done as part of a hands-on machine learning project with Apziva.  

### 💼 Business Goals:
- Accurately predict **subscribers** to the investment product.
- **Avoid calling** unlikely leads to reduce operational costs.
- Recommend **key customer segments** for call prioritization.
- Identify **top predictive features** to assist in marketing strategy.

---

## 🔁 Project Workflow

This project was tackled using a **two-model strategy**:

### ✅ 1. Pre-Call Model  
- **Goal**: Predict if a customer is likely to say "no" *before* the call is even made.  
- **Approach**: Excluded all call-related metadata (e.g., call duration, contact month).  
- **Preferred Model**: `DecisionTreeClassifier`  
- **Why**: High precision, excellent recall, strong interpretability.

### ✅ 2. Post-Call Model  
- **Goal**: Identify customers who are **likely to say "yes"** *after* the call based on call metadata.  
- **Approach**: Included features like `duration`, `contact`, and `month`.  
- **Preferred Model**: `XGBoostClassifier`  
- **Why**: Best F1 score after threshold tuning, and top-ranked feature importance aligned with business logic.

---

## 🔍 Exploratory Data Analysis (EDA)

- 📈 **Call Duration**: Strong positive relationship with subscription likelihood.
- 📅 **Months like August & December** had higher success rates.
- 💰 **Account Balance** and **Total Loans** influenced response patterns.
- 📊 **Age Grouping** revealed that younger and middle-aged customers showed lower interest.
- 🧑‍💼 **Job type and marital status** showed clear impact on decisions.

---

## ⚙️ Modeling Details

### ✨ Pre-Call Modeling Highlights

| Model              | Precision | Recall | F1 Score | Notes |
|--------------------|-----------|--------|----------|-------|
| Decision Tree      | 0.930     | 0.986  | **0.957** | Best performer |
| Random Forest      | 0.880     | 0.986  | 0.930    | Close second |
| Naive Bayes        | 0.649     | 0.993  | 0.786    | High recall, low precision |

🔍 **Important Features**:  
`age`, `balance`, `marital_status`, `education_level`  
➡️ These represent groups **less likely to subscribe**, helping avoid wasted calls.

---

### ✨ Post-Call Modeling Highlights

| Model              | Precision | Recall | F1 Score (Test) | F1 Score (Tuned) |
|--------------------|-----------|--------|-----------------|------------------|
| XGBoost            | 0.373     | 0.867  | 0.522           | **0.749** ✅ |
| Gradient Boosting  | 0.316     | 0.838  | 0.460           | - |
| Decision Tree      | 0.279     | 0.808  | 0.414           | - |

🔍 **Important Features**:  
`month_aug`, `total_loans`, `duration`, `contact_unknown`  
➡️ Likely walk-ins or well-informed clients — **excellent leads to prioritize**.

---

## 🔧 Threshold Tuning

Threshold adjustment on the post-call XGBoost classifier boosted F1 from **0.522 to 0.749** by balancing precision and recall.  
This allowed the model to more effectively identify "yes" clients despite class imbalance.

---

## 📌 Final Model Selection

✅ **Pre-Call**: `DecisionTreeClassifier` — High performance and interpretable  
✅ **Post-Call**: `XGBoostClassifier` — Excellent after threshold tuning, useful feature insights  

Stacked ensemble methods were evaluated, but **did not outperform XGBoost** and were not deployed.

---

## ✅ Recommendations

- **Train call center agents to close faster**: EDA shows longer calls increase conversion.
- **Avoid calling clients with low balance, older age, and secondary education** — they’re unlikely to subscribe.
- **Prioritize August campaigns and customers with multiple loans**.
- **Target walk-in customers (contact=unknown)** who may already be informed.

---

## 📢 Final Thoughts for Hiring Managers

This project demonstrates my ability to:

- Build real-world ML workflows from EDA to model deployment
- Handle imbalanced classification problems
- Engineer business-relevant features
- Tune, interpret, and explain models with clarity
- Translate technical results into strategic business insights

Let’s connect if you’re looking for someone who bridges the gap between data science and business decision-making.

---

## 🔗 Links

- 💻 [View the Project on GitHub](https://github.com/AlvinSMoyo/8Pl5KRkI1SP3AL13)  
- 📓 [Open Colab Notebook](https://colab.research.google.com/drive/1Y9x4k2wpe-qzrU_xJBvxd1AN6oKhHOtn?usp=sharing)  
- 🌐 [My Great Learning ePortfolio](https://www.mygreatlearning.com/eportfolio/alvin-moyo)

---
