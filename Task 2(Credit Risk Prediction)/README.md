# Credit Risk Prediction - Loan Default Analysis

## 📊 Project Overview
This project focuses on building a machine learning model to predict loan defaults using a comprehensive dataset of 20,000 loan applications. The solution helps financial institutions make data-driven lending decisions and minimize risks.

## 🎯 Task Objective
**Predict whether a loan applicant is likely to default on a loan** based on various financial and demographic features.

## Dataset
- **Size**: 20,000 records with 22 features
- **Features**: Demographic information, financial metrics, credit history, loan details
- **Target**: `loan_paid_back` (converted to `default_risk` for prediction)

## 📈 Approach

### 1. Data Understanding & Cleaning
- Comprehensive data exploration and validation
- No missing values or duplicates found
- Target variable transformation for binary classification

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis of numerical and categorical features
- Correlation analysis between features
- Default rate analysis across different segments
- Visualization of key risk factors

### 3. Feature Engineering
- Encoding of categorical variables
- Feature selection based on business relevance
- Data scaling for model compatibility

### 4. Model Development
- Three classification models implemented:
  - Logistic Regression
  - Decision Tree
  - Random Forest
- Stratified train-test split (70-30)
- Comprehensive model evaluation

### 5. Model Evaluation
- Multiple metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC
- Confusion matrix analysis
- Feature importance ranking

## 🔍 Results and Insights

### Model Performance
| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | ~0.85 | ~0.84 | ~0.86 | ~0.85 | ~0.93 |
| Decision Tree | ~0.87 | ~0.86 | ~0.88 | ~0.87 | ~0.87 |
| **Random Forest** | **~0.89** | **~0.88** | **~0.90** | **~0.89** | **~0.96** |

### Key Risk Factors Identified
1. **Credit Score**: Applicants with scores below 600 have significantly higher default rates
2. **Debt-to-Income Ratio**: Ratios above 30% substantially increase default risk
3. **Delinquency History**: Multiple delinquencies are strong predictors of default
4. **Employment Status**: Unemployed and student applicants show higher default rates
5. **Interest Rates**: Higher rates correlate with increased default probability

### Business Recommendations
1. **Credit Scoring**: Implement minimum credit score thresholds
2. **Debt Management**: Set maximum DTI ratios at 40%
3. **Risk Segmentation**: Categorize applicants into Low/Medium/High risk segments
4. **Model Deployment**: Use Random Forest for accurate default prediction
5. **Monitoring**: Regular model retraining and performance tracking

## 📁 Files Structure
- Task 2 Jupiter Notebook.ipynb # Main Jupyter notebook
- loan_dataset_20000.csv # Dataset file
- README.md # Project documentation

## Technologies Used
- Python 3.x
- Pandas, NumPy (Data manipulation)
- Matplotlib, Seaborn (Visualization)
- Scikit-learn (Machine Learning)
- Jupyter Notebook
