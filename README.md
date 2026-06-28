# Employee Attrition Prediction

This repository explores employee attrition using the IBM HR Analytics dataset. The goal is to understand why employees leave, which groups are most at risk, and what signals can help HR teams take earlier action.

## Overview

Employee attrition is a major challenge for organizations because it affects hiring costs, team stability, productivity, and retention of institutional knowledge. This project uses machine learning and exploratory data analysis to identify the most important factors linked to employee exits.

The analysis focuses on questions such as:

- Which departments and job roles show the highest attrition?
- How do income, work-life balance, and tenure relate to turnover?
- Which model gives the most useful prediction performance?
- What features matter most when estimating attrition risk?

## Dataset

The project uses the **IBM HR Analytics Employee Attrition** dataset from Kaggle:

https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

It contains 1,470 employee records with a target column, `Attrition`, indicating whether an employee stayed or left.

## What This Repository Contains

- `analysis.ipynb` — end-to-end analysis notebook
- `HR_Attrition.csv` — dataset used for the analysis
- `summary.pdf` or `summary.docx` — short business-facing summary
- `charts/` — saved visualizations from the analysis

## Analysis Workflow

### Data exploration
The notebook begins by loading and inspecting the data, checking class balance, and separating numeric and categorical features.

### Data preparation
The dataset is cleaned by removing irrelevant fields, encoding categorical variables, converting the target column to binary format, and scaling numeric features.

### Exploratory analysis
The analysis studies attrition patterns by department, job role, salary, work-life balance, and years at the company to identify meaningful trends.

### Model comparison
Several classification models are trained and compared, including:

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

### Evaluation and interpretation
The best-performing model is evaluated using precision, recall, F1-score, ROC-AUC, and confusion matrix analysis. Feature importance is then used to highlight the strongest predictors of attrition.

## Key Business Questions

This project is designed to help answer practical HR questions such as:

- Which employees are most likely to leave?
- What warning signs appear before attrition happens?
- Which departments or roles need more retention support?
- Is compensation the main reason employees leave, or are other factors more important?

## Visualizations

The notebook includes charts such as:

- Attrition by department and job role
- Monthly income comparison for employees who left vs. stayed
- Confusion matrix for the best model
- Top 10 feature importances
- ROC curve comparison across models

## Libraries Used

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Why This Project Matters

The purpose of this work is not only to predict attrition, but also to turn model results into understandable business insights that HR teams can use for retention planning and employee support.

## Getting Started

1. Download the Kaggle dataset.
2. Place the CSV file in the project folder.
3. Open `analysis.ipynb` in Jupyter Notebook or Google Colab.
4. Run the notebook from top to bottom.
5. Review the charts, model results, and business conclusions.

## Project Focus

This repository is centered on practical employee retention analysis and machine learning interpretation for HR decision-making.
