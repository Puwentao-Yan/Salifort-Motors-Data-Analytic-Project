# Why Do They Leave?
## Uncovering Employee Retention Secrets with Data

### 📊 Employee Attrition Analysis | Logistic Regression | HR Analytics

This project analyzes employee attrition using HR data from a fictional company, **Salifort Motors**, to uncover the key factors that influence whether employees leave or stay. The work was completed as the **final capstone project for the Google Advanced Data Analytics Professional Certificate**.

Rather than chasing raw prediction accuracy, the focus of this project is **interpretability and actionable business insight**, helping HR teams understand why employees leave and where interventions should be targeted.

### 🔍 Business Problem

Employee turnover is costly. Recruiting, onboarding, and lost productivity make replacing an employee significantly more expensive than retaining one.

**Stakeholder Question:**

What factors are most likely to cause an employee to leave the company?

From a modeling perspective, this is a binary classification problem. From a business perspective, it’s a decision-support problem.

**Prediction is the tool. Insight is the product.**

### 📁 Dataset Overview

The dataset contains ~15,000 employee records with the following features:

| **Feature**	| **Description** |
| ----------- | --------------- |
| satisfaction_level	| Employee-reported job satisfaction (0–1) |
| last_evaluation	| Performance review score (0–1) |
| number_project	| Number of projects |
| average_monthly_hours	| Average monthly working hours |
| time_spend_company	| Tenure (years) |
| work_accident	Work | accident indicator |
| promotion_last_5years	| Promotion indicator |
| department	| Department |
| salary	| Salary category |
| left	| Attrition outcome (target variable) |

After removing duplicates, ~16.6% of employees had left the company.

### 🧹 Data Preparation

Key preprocessing steps included:

* Removal of **3,008 duplicate rows**

* Standardized column naming (snake_case)

* **Outlier capping** for tenure using the IQR method

* One-hot encoding for salary

* **Upsampling** the minority class to address class imbalance

The goal was not perfect data, but **reliable signal without distortion**.

### 📊 Exploratory Data Analysis (EDA)

Key findings from EDA:

* No severe multicollinearity among numerical features

* Attrition clusters at **both low and high satisfaction levels**

* Workload and performance extremes increase attrition risk

* Longer tenure correlates with higher likelihood of leaving

* Salary has a strong relationship with attrition

* Department showed minimal impact and was excluded from modeling

### 🤖 Model Selection & Training

**Model used:** Logistic Regression
**Why?**

* Interpretable coefficients

* Suitable for binary classification

* Easy to communicate to non-technical stakeholders

The data was split into:

* **75% training**

* **25% testing**

### 📈 Model Performance
|**Metric**	| **Score** |
| -------- | :--: |
| Accuracy |	83% |
| Recall (Left)	| 88% |
| Precision (Left)	| 80% |

High recall was prioritized to ensure employees at risk of leaving are identified early.

### 🧠 Key Insights from Model Coefficients

* **Satisfaction dominates everything**

* **Low and medium salaries increase attrition**

* **Promotions strongly reduce attrition**

* **Longer tenure increases risk**, suggesting growth ceilings

* **Work accidents correlate with retention**

This reinforces that **engagement and career growth matter more than raw workload alone**.

### 💼 Business Recommendations

Based on the analysis:

* Track employee satisfaction continuously (not just annually)

* Re-evaluate low and medium salary bands against market benchmarks

* Create visible growth paths for long-tenured employees

* Monitor workload extremes as early burnout signals

* Use the model as an **early-warning system**, not a decision-maker

### ⚠️ Limitations & Future Work

* Logistic regression assumes linear relationships

* Upsampling may inflate performance metrics

Future improvements:

* Tree-based models (Random Forest, XGBoost)

* Cost-sensitive learning

* Time-based attrition modeling

* Richer features (role level, engagement surveys)

### 📄 Project Artifacts

* 📓 **Jupyter Notebook:**
salifort_motors_capstone_project.ipynb

* 📄 **Notebook PDF:**
salifort_motors_capstone_project.pdf

* ✍️ **Medium Blog Post:**
(https://medium.com/@yanpuwentao/why-do-they-leave-uncovering-employee-retention-secrets-with-data-8fe5ea297ab7)

### 🛠️ Tech Stack

* Python

* Pandas, NumPy

* Matplotlib, Seaborn

* Scikit-learn

### 📌 Disclaimer

This project uses a **fictional dataset and business scenario** provided by Coursera. It is intended for educational and portfolio purposes only.
