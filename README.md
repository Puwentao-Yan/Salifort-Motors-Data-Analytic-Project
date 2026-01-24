# Employee Attrition Prediction – Salifort Motors

## Project Overview
This project analyzes employee data from **Salifort Motors** to identify the key factors that contribute to employee attrition and to build a predictive model that estimates the likelihood of an employee leaving the company.

Employee turnover is costly and disruptive. Using data analysis and machine learning, this project provides data-driven insights to help the HR department improve employee retention and workforce planning.

## Business Problem
The HR department collected historical employee data but lacked clarity on:
- Why employees leave the company  
- Which factors most strongly influence attrition  
- How to proactively identify employees at risk of leaving  

**Core question:**  
> What factors are most likely to cause an employee to leave the company?

## Objectives
- Explore and clean HR employee data  
- Identify patterns and drivers of employee attrition  
- Build and evaluate a predictive classification model  
- Translate model outputs into actionable HR recommendations  

## Dataset
The dataset contains approximately **15,000 employee records** with features related to:
- Job satisfaction and performance evaluations  
- Workload and tenure  
- Promotions and work accidents  
- Department and salary level  
- Attrition status (target variable)  

## Methodology
This project follows the **PACE framework**:
- **Plan** – Understand the business context and data  
- **Analyze** – Perform exploratory data analysis (EDA) and visualizations  
- **Construct** – Train and evaluate a logistic regression model  
- **Execute** – Interpret results and propose business recommendations  

## Model Performance
A logistic regression model was trained to predict employee attrition.

- **Accuracy:** ~83%  
- **Recall (Attrition):** ~88%  
- **Precision (Attrition):** ~80%  
- **F1-score:** ~0.84  

The model performs well at identifying employees likely to leave, making it suitable as an early warning tool to support HR decision-making.

## Key Insights
- Employee satisfaction is the strongest predictor of attrition  
- Employees with low and medium salaries are significantly more likely to leave  
- Promotions substantially reduce the likelihood of attrition  
- Longer tenure and high performance evaluations may indicate burnout or external job opportunities  

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

## Ethical Considerations
- Employee privacy and data security were maintained  
- Model predictions are intended to support—not replace—human judgment  
- Results should be used to improve employee experience, not penalize individuals  

## Repository Structure
- `notebook.ipynb` – Full data analysis, visualizations, modeling, and evaluation  
- `README.md` – Project overview and high-level results  

## Notes
This project was completed as a capstone-style analysis and is intended for educational and portfolio purposes.

For detailed analysis, visualizations, and model implementation, please refer to the Jupyter notebook included in this repository.
