# synent-task6-customersegmentation-Kinari-Thummar
Customer segmentation on Mall Customer dataset — data preprocessing, K-Means clustering and cluster visualization to group customers based on behavior | Synent Technologies Internship

# Customer Segmentation Analysis

## Problem Statement
The Mall Customer dataset contains information about customers
including their age, gender, annual income and spending score.
The goal is to segment customers into distinct groups based on
their behavior using K-Means clustering to help develop
targeted marketing strategies.

## Dataset
- **Source:** [Kaggle Mall Customer Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Rows:** 200
- **Columns:** 5

## Approach

### 1. Data Preprocessing
- Renamed columns for clarity
- Checked and confirmed no missing values or duplicates
- Applied Standard Scaling before clustering

### 2. Exploratory Data Analysis
- Gender distribution
- Age distribution
- Annual income distribution
- Spending score distribution
- Correlation heatmap

### 3. Optimal Cluster Selection
- Elbow Method — identified K=5 as optimal
- Silhouette Score — confirmed K=5 with score of 0.556

### 4. K-Means Clustering
- Applied K-Means with K=5
- Visualized 2D and 3D customer segments
- Analyzed gender and age distribution per cluster

## Customer Segments Identified

| Cluster | Label | Customers | Avg Income | Avg Spending |
|---------|-------|-----------|------------|--------------|
| 0 | Average Income Average Spending | 81 | $55k | 49 |
| 1 | High Income High Spending | 39 | $86k | 82 |
| 2 | Low Income High Spending | 22 | $25k | 79 |
| 3 | High Income Low Spending | 35 | $88k | 17 |
| 4 | Low Income Low Spending | 23 | $26k | 20 |

## Key Insights
- **K=5** is the optimal number of clusters confirmed by both Elbow and Silhouette methods
- **Cluster 1** is the most valuable segment for premium marketing
- **Cluster 3** represents the biggest untapped revenue opportunity
- **Female customers** dominate all clusters except Cluster 3
- **Younger customers** tend to spend more regardless of income level

## Business Report
See [customer_segmentation_report.md](customer_segmentation_report.md)
for the complete analysis report with recommendations.

## Tools Used
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook