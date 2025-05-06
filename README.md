# 🛍️ Customer Segmentation with K-Means Clustering

This project uses **K-Means clustering** to segment customers based on their **annual income** and **spending score**. It helps uncover patterns in customer behavior to inform business strategies like targeted marketing and promotions.


## 📂 Dataset

**File:** `Mall_Customers (1).csv`  
The dataset includes:

- `CustomerID`
- `Gender`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`


## 🚀 Objectives

- Preprocess the data (standardization)
- Use the Elbow Method to find the optimal number of clusters (`k`)
- Apply K-Means clustering
- Visualize the clusters using PCA
- Evaluate cluster quality using the **Silhouette Score**
- Interpret each cluster's behavior

## 🧪 How It Works

### 1. Feature Selection

We focus on these two features for clustering:

- **Annual Income (k$)**
- **Spending Score (1–100)**

These features are standardized using `StandardScaler`.


### 2. Elbow Method

To determine the optimal number of clusters (`k`), we plot the **inertia** values for `k = 1` to `10`:

![Elbow Plot](elbow_plot.png)

> The "elbow" is observed at **k = 5**, which is selected for clustering.


### 3. Clustering & Visualization

K-Means clustering is applied with **k = 5**, and **PCA** is used to reduce the data to 2 dimensions for visualization:

![Cluster Plot](cluster_plot.png)


### 4. Evaluation

**Silhouette Score**: `0.553`

This indicates reasonably well-separated and meaningful clusters.


## 📊 Cluster Descriptions

| Cluster | Avg. Income (k$) | Avg. Spending Score | Description                        |
|---------|------------------|----------------------|------------------------------------|
| 0       | XX.X             | XX.X                 | e.g., High income, low spending    |
| 1       | XX.X             | XX.X                 | e.g., Low income, high spending    |
| 2       | XX.X             | XX.X                 | e.g., Average income and spending  |
| 3       | XX.X             | XX.X                 | e.g., High income, high spending   |
| 4       | XX.X             | XX.X                 | e.g., Low income, low spending     |

> Replace `XX.X` with actual values from the output.


## 📌 Conclusion

K-Means clustering successfully segmented mall customers into 5 groups based on income and spending habits. These insights can help businesses create **targeted campaigns** and **optimize customer engagement**.

## 📁 Files in This Repository

- `kmeans_clustering.py` — Main script
- `Mall_Customers.csv` — Dataset
- `elbow_plot.png` — Elbow method plot
- `cluster_plot.png` — Cluster visualization
- `README.md` — Project documentation

