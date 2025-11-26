# Customer Churn Prediction - Bank Customers

## 📊 Project Overview
This project focuses on predicting bank customer churn using machine learning techniques. The goal is to identify customers who are likely to leave the bank, enabling proactive retention strategies and reducing customer attrition costs.

## 🎯 Task Objective
- Predict which bank customers are likely to churn based on demographic, financial, and behavioral characteristics
- Identify key factors driving customer churn
- Provide actionable insights for customer retention strategies

## Dataset
- **Size:** 10,000 customer records with 14 features
- **Feastures:** Removed irrelevant columns, handled missing values, encoded categorical variables
- **Target Variable:** Exited (1 = Churned, 0 = Retained)

## 📈 Approach

### 1. Data Understanding & Cleaning
- **Dataset:** 10,000 customer records with 14 features
- **Target Variable:** Exited (1 = Churned, 0 = Retained)
- **Data Cleaning:** Removed irrelevant columns, handled missing values, encoded categorical variables

### 2. Exploratory Data Analysis (EDA)
- Analyzed churn distribution and class imbalance
- Investigated relationships between features and churn
- Created visualizations for key insights
- Identified correlation patterns

### 3. Feature Engineering
- Label Encoding: Gender variable
- One-Hot Encoding: Geography variable
- Feature Scaling: StandardScaler for numerical features

### 4. Model Training
- Algorithms Used:
  - Logistic Regression
  - Random Forest Classifier
- Train-Test Split: 80-20 split with stratification
- Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC

### 5. Model Evaluation & Interpretation
- Comprehensive performance comparison
- Feature importance analysis
- Business insights extraction

## 🔍 Key Results & Insights

### Model Performance
| Model |	Accuracy |	Precision	| Recall |	F1-Score	| AUC-ROC |
|-------|----------|------------|--------|------------|---------|
| Logistic Regression |	0.8120 |	0.6593 |	0.2115 |	0.3200 |	0.7631 |
| Random Forest |	0.8640 |	0.7778 |	0.4712 | 0.5870 |	0.8460 |

## Top Churn Drivers
- **Age:** Older customers (45+) significantly more likely to churn
- **Geography:** German customers have highest churn rate (32.4%)
- **Balance:** Specific balance ranges correlate with churn
- **Active Status:** Inactive members 2.5x more likely to churn
- **Number of Products:** Customers with 1 product highest churn risk

## Business Impact
- **Churn Rate:** 20.37% of customers churned
- **High-Risk Segments:** German customers aged 45+ with high balances
- **Retention Opportunity:** Model can identify 77.8% of true churn cases with precision

## 📁 File Structure
- Task 3 Jupiter Notebook.ipynb # Main Jupyter notebook
- Chuurn_Modelling.csv # Dataset file
- README.md # Project documentation

## Technologies Used
- Python 3.x
- Pandas, NumPy (Data manipulation)
- Matplotlib, Seaborn (Visualization)
- Scikit-learn (Machine Learning)
- Jupyter Notebook
