**K-Means Clustering of Mall Customers Dataset*****
Aim
` Do unsupervised learning with K-Means clustering on the Mall Customers dataset to cluster customers based upon their attributes.

🛠 Tools Used
  Python
  Pandas - to load and manipulate data
  Matplotlib - for visualizing output
  Scikit-learn - for clustering with K-Means, dimensionality reduction with PCA and evaluation metrics

📂 Dataset
  The dataset Mall_Customers.csv consists of demographic and spending data for customers.
  General columns:
      CustomerID
      Gender
      Age
      Annual Income (k$)
      Spending Score (1-100)
      
** Steps Followed**
1. Employ & Pre-process Data
  Load the data via Pandas.
  Before clustering we will only select numerical attributes.
  Standardise attributes using StandardScaler to weight all attributes equally.

2. Dimensionality Reduction (PCA - optional)
  Reduce the dataset to 2 components for visualization.
  Plot the initial characteristics of the data in 2D space.

3. Elbow Method for Optimal K
  Run K-Means for K = 2 to 10 for a number of clusters.
  Store the inertia (the sum of squared distances) against each K.
  Plot the elbow curve and visually determine optimal K.

4. Fit K-Means Clustering & Assign Clustering Labels
  Select an optimal number (subsequently to continue with an example K = 5).
  Fit KMeans to the standardised data.
  Assign customers into clusters with their clustering labels.

5. Cluster Visualisation 
  Visualise the clusters with different colours using the PCA-reduced data.
  Each colour is one cluster.

6. Evaluation
  Calculate the Silhouette Score to measure how well customers are clustered.
      Score ranges from -1 to 1.
      Higher values indicate better separation between clusters.
