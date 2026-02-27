# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1: Initialize Parameters

Load customer dataset (e.g., Age, Income, Spending Score).

Choose number of clusters 
𝐾
K.

Randomly initialize 
𝐾
K centroids.

Step 2: Assign Clusters

For each customer data point:

Compute distance (e.g., Euclidean distance) to all centroids.

Assign the customer to the nearest centroid.

Step 3: Update Centroids

For each cluster:

Compute the new centroid by taking the mean of all data points assigned to that cluster.

Step 4: Repeat Until Convergence

Repeat Steps 2 and 3 until:

Centroids no longer change significantly, or

Maximum number of iterations is reached.

Output final clusters for customer segmentation.

## Program:
```
/*
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans
data = pd.read_csv("Mall_Customers.csv")
X = data[['Annual Income (k$)', 'Spending Score (1-100)']]
print(data.head())
kmeans = KMeans(n_clusters=5, random_state=42)
y_kmeans = kmeans.fit_predict(X)


data['Cluster'] = y_kmeans

print("\nClustered Data:")
print(data.head())


plt.figure()
plt.scatter(X[y_kmeans == 0]['Annual Income (k$)'], 
            X[y_kmeans == 0]['Spending Score (1-100)'], label='Cluster 0')

plt.scatter(X[y_kmeans == 1]['Annual Income (k$)'], 
            X[y_kmeans == 1]['Spending Score (1-100)'], label='Cluster 1')

plt.scatter(X[y_kmeans == 2]['Annual Income (k$)'], 
            X[y_kmeans == 2]['Spending Score (1-100)'], label='Cluster 2')

plt.scatter(X[y_kmeans == 3]['Annual Income (k$)'], 
            X[y_kmeans == 3]['Spending Score (1-100)'], label='Cluster 3')

plt.scatter(X[y_kmeans == 4]['Annual Income (k$)'], 
            X[y_kmeans == 4]['Spending Score (1-100)'], label='Cluster 4')

plt.scatter(kmeans.cluster_centers_[:,0], 
            kmeans.cluster_centers_[:,1], 
            s=200, label='Centroids')

plt.title("Customer Segmentation using K-Means")
plt.xlabel("Annual Income (k$)")
plt.ylabel("Spending Score (1-100)")
plt.legend()
plt.show()
Developed by:VARUNA.R
RegisterNumber:25004445
*/
```

## Output:
<img width="747" height="137" alt="Screenshot 2026-02-27 140509" src="https://github.com/user-attachments/assets/799ab3c9-bd74-4f2b-bcb6-d58bc107eb53" />
<img width="748" height="328" alt="Screenshot 2026-02-27 140531" src="https://github.com/user-attachments/assets/853f7285-64cd-4044-bc0d-08f97311ffd2" />
<img width="805" height="570" alt="Screenshot 2026-02-27 140541" src="https://github.com/user-attachments/assets/f61e81f7-7527-4df4-8094-73a76302b644" />





## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
