# Bank Marketing Campaign - Term Deposit Subscription Prediction

## 📋 Project Overview
This project focuses on predicting whether a bank customer will subscribe to a term deposit based on marketing campaign data. Using machine learning techniques, we analyze customer demographics, financial information, and campaign interactions to build predictive models that can optimize marketing strategies and improve campaign efficiency.

## 🎯 Business Objective
Help banks optimize their marketing campaigns by identifying customers most likely to subscribe to term deposits, thereby:
- Improving campaign success rates
- Reducing marketing costs
- Enhancing customer experience through targeted communications
- Increasing return on investment (ROI)

## 📊 Dataset
**Source**: UCI Machine Learning Repository - Bank Marketing Dataset  
**Size**: 11,162 samples with 16 features  
**Target Variable**: `deposit` (yes/no) - whether customer subscribed to term deposit

### Key Features:
- **Demographic**: age, job, marital status, education
- **Financial**: balance, default, housing loan, personal loan
- **Campaign**: contact type, day, month, duration, campaign contacts
- **Historical**: previous campaign outcomes, days since last contact

## 🛠️ Technical Implementation
### Technologies Used:
- **Python 3.x**
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, SHAP (for interpretability)
- **Machine Learning Models**: Logistic Regression, Random Forest, Gradient Boosting
- **Evaluation Metrics**: Accuracy, F1-Score, ROC-AUC, Confusion Matrix

### Project Structure:
bank-deposit-prediction/
│
├── bank.csv # Dataset
├── Term_Deposit_Prediction.ipynb # Main Jupyter Notebook
├── requirements.txt # Python dependencies
├── README.md # This file
│
├── models/
│ └── best_deposit_prediction_model.joblib # Saved best model
│
├── outputs/
│ ├── project_summary.txt # Project summary (UTF-8)
│ ├── project_summary_simple.txt # ASCII-only summary
│ ├── project_metrics.csv # Performance metrics
│ └── visualizations/ # Generated plots and charts


## 📈 Methodology
### 1. Data Exploration & Cleaning
- **Data Quality Assessment**: Checked for missing values, duplicates, and inconsistencies
- **Data Cleaning**: Handled 'unknown' values by replacing with mode
- **Exploratory Analysis**: Visualized distributions, correlations, and patterns

### 2. Feature Engineering & Preprocessing
- **Target Encoding**: Converted 'yes/no' to binary (1/0)
- **Feature Scaling**: Standardized numerical features
- **Categorical Encoding**: One-hot encoding for categorical variables
- **Data Splitting**: 80% training, 20% testing with stratification

### 3. Model Development
Three classification algorithms were implemented and compared:
- **Logistic Regression** (Baseline model)
- **Random Forest** (Ensemble method)
- **Gradient Boosting** (Advanced ensemble)

### 4. Model Evaluation & Selection
- **Performance Metrics**: Accuracy, Precision, Recall, F1-Score, ROC-AUC
- **Cross-validation**: 5-fold cross-validation for robustness
- **Model Comparison**: Side-by-side evaluation using multiple metrics

### 5. Model Interpretability (XAI)
- **Feature Importance**: Analyzed which features most influence predictions
- **SHAP Values**: Explained individual predictions and feature contributions
- **Business Insights**: Translated model outputs into actionable recommendations

## 🏆 Results
### Model Performance Comparison:

| Model | Accuracy | F1-Score | ROC-AUC | Best For |
|-------|----------|----------|---------|----------|
| Random Forest | ~89% | ~0.88 | ~0.95 | Production |
| Gradient Boosting | ~88% | ~0.87 | ~0.94 | Competitions |
| Logistic Regression | ~87% | ~0.86 | ~0.88 | Baseline |

**Best Model**: Random Forest classifier with **89% accuracy** and **0.88 F1-Score**

### Key Findings:
1. **Most Important Features**:
   - Duration of last contact (strongest predictor)
   - Customer age
   - Account balance
   - Number of campaign contacts
   - Housing loan status

2. **High-Probability Customer Profile**:
   - Age: 30-50 years
   - Occupation: Admin, Management, Technician
   - Education: Tertiary level
   - Financial: Higher balance, no housing loan
   - Campaign: Fewer contacts (<3), longer call duration (>5 minutes)

## 💡 Business Insights & Recommendations
### Target Segmentation Strategy:
- **Primary Focus**: Admin/Management professionals aged 30-50 with higher balances
- **Secondary Focus**: Technicians, tertiary-educated customers
- **Avoid**: Customers with >3 previous contacts, housing loan holders

### Campaign Optimization:
1. **Contact Strategy**: Limit to 2-3 contacts per customer
2. **Call Quality**: Aim for >5 minute conversations
3. **Contact Method**: Prefer cellular over telephone
4. **Timing**: Schedule campaigns in May-June for best results

### Resource Allocation:
- Use model scoring to prioritize high-probability customers
- Allocate 60% budget to high-probability, 30% medium, 10% low segments
- Focus on customers with balance > median balance of subscribers

### Expected ROI Impact:
- **25% improvement** in conversion rates expected
- **40% reduction** in wasted contacts
- **Significant cost savings** with targeted approach

## 🚀 Getting Started
### Prerequisites:
- Python 3.7+
- Jupyter Notebook
- Required libraries (see requirements.txt)

##📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

##🙏 Acknowledgments
- UCI Machine Learning Repository for the dataset
- Scikit-learn team for the excellent machine learning library
- SHAP developers for model interpretability tools
- Open-source community for various Python libraries

##📞 Contact & Support
For questions, suggestions, or collaboration opportunities:
Email: mtahabulc1922example.com
LinkedIn: www.linkedin.com/in/m-taha-nazeef-673912282
