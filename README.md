# SmartCart Customer Segmentation

## Project Overview

SmartCart Customer Segmentation is an Unsupervised Machine Learning project that identifies distinct customer groups based on demographic information, purchasing behavior, income, and spending patterns.

The objective is to understand customer behavior and develop targeted marketing strategies for different customer segments.

## Dataset

- Total customer records: 2,240
- Total columns: 22
- Missing values: 24 in the Income column

The dataset includes customer demographics, income, purchase history, spending habits, and campaign response information.

## Technologies Used

- Python
- JupyterLab
- Pandas
- Matplotlib
- Seaborn
- NumPy
- Scikit-learn
- Kneed

## Project Workflow

### 1. Data Preprocessing

- Identified missing values.
- Handled missing Income values using median imputation.
- Removed irrelevant columns.
- Detected and filtered outliers in Age and Income.

### 2. Feature Engineering

Created additional features:

- Age
- Customer Tenure (Days)
- Total Spending
- Total Children

Also grouped Education and Marital Status into broader categories for customer profiling.

### 3. Exploratory Data Analysis

- Analyzed customer demographics and purchasing behavior.
- Examined distributions and outliers.
- Used correlation heatmaps to identify relationships between numerical features.

### 4. Encoding and Scaling

- Applied One-Hot Encoding to categorical features.
- Used StandardScaler to standardize numerical features.

### 5. Dimensionality Reduction

Applied Principal Component Analysis (PCA) to reduce the feature space.

Explored both 2D and 3D representations of customer data.

### 6. Optimal Cluster Selection

Used two methods to determine the number of clusters:

- Elbow Method (WCSS)
- Silhouette Score

Selected four clusters based on the combined analysis.

### 7. Clustering Algorithms

Implemented and explored:

- K-Means Clustering
- Agglomerative Clustering (Ward Linkage)

### 8. Customer Segmentation and Analysis

Identified four customer segments:

| Cluster | Customer Segment | Marketing Strategy |
|---|---|---|
| 0 | Family Shoppers | Discounts and coupons |
| 1 | Premium Customers | Loyalty programs |
| 2 | Budget-conscious Customers | Sales and promotional offers |
| 3 | High-value Singles | Premium and personalized services |

## Key Findings

- Customer purchasing behavior varies with income and spending patterns.
- Customers with higher income generally demonstrate higher spending.
- Customers with more children tend to show different purchasing patterns.
- Four customer segments provide distinct opportunities for targeted marketing.

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Navigate to the project directory:

   ```bash
   cd smartcart-customer-segmentation
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch JupyterLab:

   ```bash
   jupyter lab
   ```

5. Open `smart_clustering_project.ipynb` and execute the notebook.

## Project Structure

```text
smartcart-customer-segmentation/
│
├── smart_clustering_project.ipynb
├── smartcart_customers.csv
├── README.md
├── requirements.txt
└── .gitignore
```

## Future Improvements

- Experiment with additional clustering algorithms.
- Improve cluster validation.
- Develop an interactive customer segmentation dashboard.
- Explore personalized marketing recommendations.

---

**Note:** This project is intended for educational and analytical purposes.