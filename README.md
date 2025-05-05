# Customer Segmentation using K-Means Clustering

## 📌 Overview
This project applies unsupervised machine learning techniques to perform **customer segmentation**, a core task in data mining. The primary objective is to identify distinct groups within a customer base based on behavioral and demographic data, allowing businesses to tailor marketing strategies, improve customer service, and enhance product targeting.

Using the **K-Means Clustering** algorithm, we discover natural groupings within the data. Dimensionality reduction via **PCA (Principal Component Analysis)** is employed to visualize the resulting clusters and validate separation quality.

---

## 🧠 Objective

The main goal is to:

- Explore and preprocess customer data.
- Apply **K-Means Clustering** to segment customers.
- Use the **Elbow Method** to determine the optimal number of clusters.
- Visualize and interpret clusters using **PCA**.
- Derive insights that can inform business decision-making.

---

## 📁 Dataset Description

The dataset used is a customer dataset (likely from a mall or e-commerce platform) and typically includes features such as:

| Column Name        | Description                            |
|--------------------|----------------------------------------|
| `CustomerID`       | Unique customer identifier             |
| `Gender`           | Gender of the customer (Male/Female)   |
| `Age`              | Age of the customer                    |
| `Annual Income`    | Annual income (in $1000s)              |
| `Spending Score`   | Score assigned based on customer spending behavior |

---

## 🔧 Technologies Used

- Python 3.x
- Jupyter Notebook
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 📊 Data Preprocessing

- **Handling Categorical Data**: Gender is encoded using label encoding.
- **Feature Scaling**: Applied `StandardScaler` to normalize data.
- **Null Value Check**: Verified dataset cleanliness (no missing values).
- **Feature Selection**: Age, Income, and Spending Score were selected for clustering.

---

## 📈 Methodology

### 1. **Exploratory Data Analysis (EDA)**
Performed EDA using boxplots, distributions, and pair plots to understand relationships and spot outliers.

### 2. **Elbow Method**
Used to determine the optimal number of clusters (`k`) by plotting Within-Cluster-Sum-of-Squares (WCSS) for `k = 1 to 10`.

### 3. **K-Means Clustering**
K-Means algorithm was applied using the optimal `k`. The resulting cluster labels were appended to the original data.

### 4. **Dimensionality Reduction (PCA)**
To visualize high-dimensional clusters in 2D, PCA was applied. Scatter plots highlight the separation of clusters.

---

## 📌 Results

- Optimal clusters (`k`) selected using the **Elbow method** (e.g., `k = 5`).
- **Cluster Visualization** clearly shows well-separated groups in PCA-reduced space.
- Each cluster represents a distinct customer persona (e.g., high spenders, young savers, low-income low spenders, etc.).

---

## 💡 Business Insights

- The clustering reveals **demographic and behavioral segmentation** of customers.
- Marketing strategies can be customized per group:
  - High-income, low-spending: Upsell or loyalty programs
  - Low-income, high-spending: Promotions or budget products
  - Young, high-spending: Trend-focused campaigns

---

## 📘 Conclusion

This project successfully demonstrates the **application of K-Means clustering for customer segmentation**, a vital use case in data mining. Through careful preprocessing, algorithmic tuning, and visualization, the model uncovers hidden structures in customer data, allowing actionable business intelligence.

---
