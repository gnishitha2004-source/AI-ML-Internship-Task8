# 🌀 Task 8: K-Means Clustering

## 📌 Objective
Perform **unsupervised learning** using **K-Means clustering** to group data into clusters, visualize results, and evaluate clustering performance.

---

## 🛠 Tools & Libraries
- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## 📂 Dataset
For demonstration, we used the **Iris dataset** (available in Seaborn library).  
Alternatively, you can use the **Mall Customers dataset** from Kaggle:  
👉 [Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

## 🚀 Steps Performed
1. Imported required libraries.  
2. Loaded the dataset into Pandas DataFrame.  
3. Preprocessed the data: selected numeric features & standardized them.  
4. Applied the **Elbow Method** to determine the optimal number of clusters (K).  
5. Trained the **K-Means model** with the chosen K.  
6. Evaluated performance using **Silhouette Score**.  
7. Used **PCA** to reduce dimensions and visualize clusters in 2D space.  

---

## 📊 Results
- **Optimal K**: 3 (from elbow curve for Iris dataset)  
- **Silhouette Score**: ~0.55 (indicating fairly good clustering)  

### Elbow Method Plot
*(Insert your plot screenshot here)*

### Cluster Visualization (PCA Projection)
*(Insert your PCA visualization screenshot here)*

---

## 📜 How to Run
1. Open [Google Colab](https://colab.research.google.com/).  
2. Copy-paste the provided Python code into a new Colab notebook.  
3. Run each cell step by step.  
4. Upload dataset if using **Mall_Customers.csv**.  
5. View results: inertia (Elbow method), silhouette score, and cluster visualization plots.  

---

## ❓ Interview Questions & Answers

**1. How does K-Means clustering work?**  
It partitions data into *k* clusters by assigning points to the nearest centroid and updating centroids iteratively until convergence.

**2. What is the Elbow Method?**  
It is used to determine the optimal number of clusters by plotting inertia vs. K and finding the "elbow" point where the decrease slows down.

**3. What are the limitations of K-Means?**  
- Sensitive to initialization  
- Requires K in advance  
- Struggles with irregular shapes or varying cluster densities  

**4. How does initialization affect results?**  
Poor initialization may cause convergence to suboptimal clusters. The `k-means++` method improves initialization.

**5. What is inertia in K-Means?**  
The sum of squared distances of data points to their assigned cluster center. Lower inertia means better clustering.

**6. What is Silhouette Score?**  
It measures how well clusters are separated. Score ranges from -1 (poor) to +1 (ideal).  

**7. How do you choose the right number of clusters?**  
Methods: Elbow Method, Silhouette Score, Gap Statistics, or domain knowledge.  

**8. Difference between clustering and classification?**  
- **Clustering**: Unsupervised, groups unlabeled data.  
- **Classification**: Supervised, assigns predefined labels.  
