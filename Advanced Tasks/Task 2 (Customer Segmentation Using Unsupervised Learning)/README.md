 # 🛍️ Mall Customer Segmentation Project

## 📋 Project Overview
This project segments mall customers based on their spending habits using unsupervised learning techniques (K-Means clustering) to help develop targeted marketing strategies.

## 🎯 Objective
To identify distinct customer segments from the Mall Customers dataset based on spending patterns and demographics, then propose tailored marketing strategies for each segment.

## 📊 Dataset
- **Source**: Mall Customers Dataset
- **Records**: 200 customers
- **Features**: 
  - CustomerID: Unique identifier
  - Genre: Gender (Male/Female)
  - Age: Customer's age
  - Annual Income (k$): Yearly income in thousands
  - Spending Score (1-100): Mall's assessment of spending behavior

## 🛠️ Technologies Used
- Python 3.x
- Pandas & NumPy for data manipulation
- Scikit-learn for machine learning
- Matplotlib & Seaborn for visualization
- Jupyter Notebook for interactive analysis

## 📁 Project Structure
mall-customer-segmentation/
├── Mall_Customers.csv # Original dataset
├── mall_customer_segmentation.ipynb # Main Jupyter notebook
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── mall_customers_clustered.csv # Results with cluster labels
├── cluster_profiles.csv # Cluster statistics
└── marketing_strategies_summary.txt # Marketing recommendations


## 🚀 Implementation Steps

### 1. Data Exploration & Preprocessing
- Load and explore dataset
- Handle missing values
- Feature engineering
- Statistical analysis

### 2. Exploratory Data Analysis (EDA)
- Visualize distributions
- Correlation analysis
- Gender-based analysis
- Age vs Spending patterns

### 3. Feature Selection & Scaling
- Select relevant features (Annual Income & Spending Score)
- Standardize features for clustering

### 4. K-Means Clustering
- Determine optimal k using Elbow Method
- Apply K-Means algorithm
- Validate with silhouette scores

### 5. Visualization
- 2D cluster visualization
- PCA for dimensionality reduction
- 3D visualization with Age, Income, Spending Score

### 6. Cluster Analysis
- Profile each segment
- Analyze characteristics
- Identify patterns

### 7. Marketing Strategy Development
- Create targeted strategies for each segment
- Propose actionable recommendations
- Estimate business impact

## 📈 Results

### Customer Segments Identified:

1. **Cluster 0**: High Income, Low Spenders
   - Conservative affluent customers
   - Focus on premium services

2. **Cluster 1**: Average Spenders
   - Balanced income and spending
   - Target with promotions

3. **Cluster 2**: High Income, High Spenders
   - VIP customers
   - Exclusive offers

4. **Cluster 3**: Low Income, High Spenders
   - Trend-conscious youth
   - Affordable luxury

5. **Cluster 4**: Low Income, Low Spenders
   - Budget-conscious
   - Value-focused offers

## 📊 Key Insights
- 5 distinct customer segments identified
- Clear correlation between income and spending patterns
- Younger customers show different spending behaviors
- Significant opportunity for personalized marketing

## 💼 Business Impact
- Personalized marketing campaigns
- Improved customer retention
- Optimized inventory management
- Increased marketing ROI


## Instructions to Use:

1. **Create the files**:
   - Save the Python code as `mall_customer_segmentation.ipynb`
   - Save the requirements as `requirements.txt`
   - Save the README as `README.md`
   - Keep your `Mall_Customers.csv` in the same folder

2. **Set up the environment**:
   ```bash
   pip install -r requirements.txt

## 👤 Author
**Muhammad Taha**

## 📞 Contact & Support
For questions, suggestions, or collaboration opportunities:
- GitHub: [@mtahanazeef](https://github.com/mtahanazeef)
- Email: mtahabulc1922example.com
- LinkedIn: www.linkedin.com/in/m-taha-nazeef-673912282
