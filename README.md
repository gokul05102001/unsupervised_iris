# Clustering Analysis of the Iris Dataset

## Overview
This repository implements clustering techniques on the Iris dataset using two popular algorithms: KMeans Clustering and Hierarchical Clustering. The goal is to apply these unsupervised machine learning techniques to identify potential groupings (clusters) within the dataset.

## Dataset
The Iris dataset is a classic dataset in machine learning that contains 150 observations of iris flowers, with 4 features (sepal length, sepal width, petal length, and petal width) for each observation. The dataset is originally labeled with the species of each flower, but for this clustering task, the species label is excluded.

## Steps

### 1. Loading and Preprocessing
- The Iris dataset is loaded from the sklearn library.
- The species column is dropped to focus on clustering the data based on the features.

### 2. Clustering Algorithms
Two clustering algorithms are applied:

#### A) KMeans Clustering
- KMeans is a centroid-based clustering algorithm that partitions the dataset into a predefined number of clusters.
- The algorithm iteratively assigns each data point to the nearest centroid and refines the centroids to minimize variance within the clusters.
- The number of clusters is set to 3 (since the Iris dataset has 3 species).

#### B) Hierarchical Clustering
- Hierarchical clustering builds a hierarchy of clusters based on their similarity.
- Agglomerative hierarchical clustering is used, where each data point starts as its own cluster, and the closest clusters are merged iteratively.
- A dendrogram is plotted to visualize the clustering hierarchy.

### 3. Visualizations
- For both KMeans and Hierarchical clustering, scatter plots are generated using the first two features (sepal length and sepal width) to visualize the clusters.
- A dendrogram is also plotted for the Hierarchical clustering method.

