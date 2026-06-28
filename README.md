# Employee Attrition Prediction

This repository contains a Jupyter Notebook project focused on building a machine learning system to predict employee attrition using HR analytics data. The project explores which factors are associated with employees leaving a company and turns those findings into practical HR insights.

## Project Goal

The goal of this project is to answer a business-critical question:

> **Which employees are most likely to leave, and why?**

Using the IBM HR Analytics Employee Attrition dataset, the notebook walks through data cleaning, exploratory data analysis, preprocessing, model training, evaluation, and business recommendations.

## Business Problem

Every company loses employees, but losing the wrong employees at the wrong time can be expensive. Attrition creates costs related to:

- Hiring and onboarding
- Training and ramp-up time
- Lower productivity
- Team disruption and morale issues

This project helps HR teams identify attrition risk early so they can take action before valuable employees leave.

## Dataset

The notebook uses the **IBM HR Analytics Employee Attrition** dataset from Kaggle:

- **Dataset link:** https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
- **File name:** `WA_Fn-UseC_-HR-Employee-Attrition.csv`
- **Rows:** 1,470
- **Target column:** `Attrition` (`Yes` / `No`)

## What This Notebook Covers

### 1. Data Loading & Exploration
- Load the CSV file with Pandas
- Preview the dataset
- Check rows and columns
- Measure class balance for attrition
- Identify numeric and categorical columns

### 2. Data Cleaning & Preprocessing
- Check and handle missing values
- Remove irrelevant or constant columns such as:
  - `EmployeeNumber`
  - `Over18`
  - `StandardHours`
- Convert `Attrition` to binary format (`Yes` → `1`, `No` → `0`)
- Apply One-Hot Encoding to categorical variables
- Scale numeric features with `StandardScaler`

### 3. Exploratory Data Analysis
The notebook analyzes attrition patterns across:
- Department
- Job Role
- Monthly Income
- Work-Life Balance
- Years at Company

It also highlights key business patterns and retention risks.

### 4. Model Building & Comparison
Three classification models are trained and compared:
- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

The project uses `class_weight='balanced'` to address class imbalance.

### 5. Model Evaluation
Each model is evaluated using:
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

The best model is then used to extract feature importance and identify the strongest drivers of attrition.

### 6. Visualization
Expected charts include:
- Attrition by Department and Job Role
- Monthly Income comparison for employees who left vs stayed
- Confusion matrix heatmap
- Feature importance chart
- ROC curve comparison

### 7. HR Insights & Recommendations
The notebook concludes with plain-language business recommendations for HR leaders, including:
- Top factors influencing attrition
- Departments or roles to prioritize
- Practical retention actions
- Model limitations

## Repository Contents

This repository is intended to include:

- `analysis.ipynb` — full notebook with all analysis and modeling steps
- `HR_Attrition.csv` — dataset used for the project
- `summary.pdf` or `summary.docx` — non-technical business summary for HR leadership
- `charts/` — saved visualizations as `.png` files

## Recommended Project Structure

```text
EmployeeAttrition_[YourName]/
├── analysis.ipynb
├── HR_Attrition.csv
├── summary.pdf
└── charts/
    ├── attrition_by_department.png
    ├── attrition_by_job_role.png
    ├── income_boxplot.png
    ├── confusion_matrix.png
    ├── feature_importance.png
    └── roc_curve.png
```

## Libraries Used

- Python 3.x
- Jupyter Notebook / Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run

1. Download the Kaggle dataset.
2. Place the CSV file in the project folder.
3. Open `analysis.ipynb` in Jupyter Notebook or Google Colab.
4. Run the notebook cells in order.
5. Review the charts, model results, and final HR recommendations.

## Key Questions This Project Answers

- What is the attrition rate in the company?
- Which departments and job roles have the highest turnover?
- Does salary strongly influence attrition?
- How does work-life balance affect employee retention?
- Which model best predicts attrition?
- What features are most important in predicting exits?

## Deliverable

The final submission should be a ZIP file containing the completed folder, along with the notebook link submitted through the provided form.

## Note

This project is designed not just to build a model, but to translate data science into business language that HR stakeholders can understand and act on.
