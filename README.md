# 🛍️ Customer Segmentation – K-Means Clustering

## 📌 Objective
Segment mall customers into distinct groups based on their annual income and spending behavior using **K-Means Clustering**.

---

## 📁 Dataset
- **Source**: [Mall Customer Segmentation Dataset on Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **File Used**: `Mall_Customers.csv`

---

## 🛠 Tools Used
- Python
- Pandas, NumPy
- Scikit-learn (KMeans, StandardScaler, silhouette_score)
- Seaborn, Matplotlib

---

## ✅ Steps Performed

### 1. Data Preparation
- Removed `CustomerID` as it's irrelevant to clustering
- Converted `Gender` to numerical (Male = 0, Female = 1)
- Selected key features: `Annual Income (k$)` and `Spending Score (1–100)`

### 2. Feature Scaling
- Used `StandardScaler` to normalize features before applying K-Means

### 3. Elbow Method to Choose K
- Plotted inertia vs. number of clusters
- **Optimal K = 5** (based on the 'elbow' point)

### 4. K-Means Clustering
- Trained `KMeans(n_clusters=5)`
- Assigned cluster labels to each customer

### 5. Visualization
- Used scatter plot to visualize clusters based on income and spending score

### 6. Evaluation with Silhouette Score
- **Silhouette Score**: `0.555`
  - Indicates **well-separated** and **cohesive** clusters

---

## 📊 Key Learnings

- K-Means is an unsupervised algorithm that groups data based on similarity
- Scaling features is essential for distance-based algorithms like K-Means
- The **Elbow Method** helps select the right number of clusters (K)
- The **Silhouette Score** measures how well each point fits into its cluster


## 📝 Submission
This project was completed as part of the **AI & ML Internship**  
**Task 8: K-Means Clustering – Customer Segmentation**

