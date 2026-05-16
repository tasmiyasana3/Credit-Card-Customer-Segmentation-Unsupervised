# Customer Segmentation using Unsupervised Learning

Unsupervised Machine Learning project focused on customer segmentation for AllLife Bank using clustering techniques such as K-Means and Hierarchical Clustering.

This project analyses customer banking behaviour, credit usage patterns, and engagement channels to identify meaningful customer groups. The objective is to help the bank improve personalised marketing strategies and enhance customer service delivery.

---

## Project Overview

AllLife Bank aims to improve market penetration and customer engagement by understanding customer behaviour patterns. Using unsupervised learning techniques, this project segments customers based on:
- Credit card usage
- Credit limits
- Bank visits
- Online activity
- Customer service calls

The project helps identify distinct customer profiles for targeted marketing campaigns and operational improvements.

---

## Business Objective

The goal of this project is to:
- Segment customers into meaningful groups
- Identify high-value and digitally active customers
- Understand customer engagement behaviour
- Improve customer service strategy
- Support personalised marketing and upselling opportunities

---

## Dataset Information

The dataset contains banking customer behaviour and financial attributes.

### Dataset Size
- **660 rows**
- **7 columns**

### Features
- `Avg_Credit_Limit`
- `Total_Credit_Cards`
- `Total_visits_bank`
- `Total_visits_online`
- `Total_calls_made`

### Dropped Columns
- `Sl_No`
- `Customer Key`

These columns were removed because they were unique identifiers and not useful for clustering.

---

## Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Yellowbrick
- Jupyter Notebook

---

## Exploratory Data Analysis (EDA)

### Key Insights

- Customers with higher credit limits generally owned more credit cards
- High-credit customers preferred online banking and rarely contacted support
- Customers with lower credit limits relied more on branch visits and phone calls
- Strong negative relationship observed between:
  - Bank visits and online visits
  - Credit cards and customer calls
- Digitally active customers showed higher creditworthiness
- Customers were clearly divided into:
  - Branch-focused users
  - Digitally engaged users

---

## Data Preprocessing

### Steps Performed
- Removed duplicate records
- Dropped identifier columns
- Checked missing values
- Outlier detection using:
  - Boxplots
  - IQR Method
- Winsorization for extreme outliers
- Feature scaling using StandardScaler
- Feature engineering

---

## Feature Engineering

New behavioural features were created to improve clustering quality and customer understanding.

These engineered features helped capture:
- Customer engagement intensity
- Digital banking preference
- Credit behaviour patterns

---

## Clustering Techniques Used

### 1. K-Means Clustering
Applied K-Means clustering to identify customer groups based on behavioural patterns.

#### Methods Used
- Elbow Method
- Silhouette Score Analysis
- Cluster Profiling

---

### 2. Hierarchical Clustering
Hierarchical clustering was applied to compare segmentation quality and cluster structure.

#### Methods Used
- Dendrogram Analysis
- Linkage Methods Comparison
- Cophenetic Correlation
- Silhouette Score Evaluation

---

## Dimensionality Reduction

### PCA (Principal Component Analysis)

PCA was used for:
- Dimensionality reduction
- Cluster visualisation
- Better interpretation of customer groups

---

## Final Model Comparison

Both clustering approaches were compared using:
- Silhouette Score
- Cluster separation
- Cluster interpretability
- Business relevance

### Conclusion
K-Means clustering provided:
- Better cluster separation
- More interpretable customer groups
- Stronger business applicability

---

## Customer Segments Identified

### High-Value Digital Customers
- High credit limits
- Multiple credit cards
- High online activity
- Low branch visits and customer calls

### Traditional Banking Customers
- Frequent branch visits
- Lower digital engagement
- Moderate credit limits

### Support-Dependent Customers
- High customer support calls
- Lower credit limits
- Lower online engagement

---

## Business Recommendations

- Target digitally active customers with premium banking products
- Improve online banking services for traditional customers
- Optimise customer support operations for high-call segments
- Create personalised marketing campaigns for each customer segment
- Encourage digital adoption among branch-focused users

---

## Project Structure

- `UnsupervisedLearning_BUSINESSREPORT_TS_pdf compressed.pdf` — Detailed business report
- `UnsupervisedLearningProject_TS.ipynb` — Complete implementation notebook
- `Credit Card Customer Data.xlsx— Complete dataset file
- `README.md` — Project documentation

---

## Author

Tasmiya Sana

---

## Conclusion

This project demonstrates how unsupervised learning techniques can help banks better understand customer behaviour and segment users into meaningful groups. By leveraging clustering algorithms, businesses can improve customer engagement, optimise service delivery, and create data-driven marketing strategies.
