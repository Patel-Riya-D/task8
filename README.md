# task8
# 🎯 Customer Segmentation Using K-Means Clustering

Welcome to this project where we apply **K-Means Clustering** to segment customers based on their demographics and spending behavior using the Mall Customer dataset.

---

## 📦 Dataset

- **Source**: Kaggle – Mall Customer Segmentation
- **Features Used**: Gender, Age, Annual Income, Spending Score

---

## 🧠 What is K-Means Clustering?

K-Means is an **unsupervised machine learning algorithm** that groups data into clusters based on similarity. It works by:

1. Selecting `K` cluster centers (centroids)
2. Assigning each point to the nearest centroid
3. Recomputing centroids until convergence

---

## 🚀 Steps Performed

- Loaded and cleaned the dataset
- Encoded gender values (Male → 0, Female → 1)
- Applied PCA for 2D visualization
- Used **Elbow Method** to choose optimal `K`
- Fitted **K-Means model**
- Visualized clusters
- Evaluated results using **Silhouette Score**

---

## 🔄 What is PCA?

**Principal Component Analysis (PCA)** is a technique used to **reduce the number of features** while preserving as much **variation (information)** in the data as possible.

In this project, we used PCA to:
- Convert high-dimensional data into **2D for visualization**
- Help visualize **clusters clearly** on a 2D plot

📌 PCA makes it easier to **see patterns and clusters** by projecting the data into 2 main components.

---

## 📉 Elbow Method :

The Elbow Plot showed that **K = 4 or 5** is optimal, where inertia (within-cluster distance) drops significantly and then levels off.

📌 _This means adding more clusters beyond this point doesn’t improve clustering much._

![image](https://github.com/user-attachments/assets/ccefe6dd-2642-4b75-83f1-f84c5ab2ae4a)


---

## 🎨 Cluster Plot :

PCA-based 2D visualization showed **visibly separated groups**, indicating meaningful clusters of customers based on age, income, and spending habits.

📌 _Color-coded clusters make it easy to understand customer groups visually._


![image](https://github.com/user-attachments/assets/58bd5d90-12b6-4551-a8a6-859e0a5e7892)

---

## 📈 Silhouette Score: `0.406`

- **What it means**: Moderate clustering quality
- ✅ Clusters have some separation
- 🔁 Could be improved with feature scaling or different K

---

## 📊 Silhouette Scores for Different K

To determine the best number of clusters, I computed Silhouette Scores for different values of K:

| K (Clusters) | Silhouette Score |
|--------------|------------------|
| 2            | 0.332            |
| 3            | 0.335            |
| 4            | 0.405            |
| 5            | 0.357            |
| 6            | 0.415            |

📌 **Best Score:** `K = 4` gave the highest Silhouette Score of **0.405**, suggesting 4 is the most suitable number of clusters.

---



---

## 🛠 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 📂 Repository Structure

