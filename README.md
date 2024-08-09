# PRODIGY_ML_02


# K-means Clustering for Customer Segmentation

## Overview
This project demonstrates the application of the K-means clustering algorithm to segment customers of a retail store based on their purchase history. The dataset used for this analysis contains features such as Age, Annual Income, and Spending Score. The goal is to identify distinct customer groups to aid in targeted marketing strategies.
Dataset

The dataset used for this project is the Mall Customer Segmentation Dataset from Kaggle. It contains information about customers, including their Age, Annual Income, and Spending Score.

    Dataset Link: [Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

# K-means Clustering Algorithm
## Algorithm Description

K-means clustering is an iterative algorithm used to partition a dataset into k distinct, non-overlapping subsets or clusters. The main objective is to minimize the variance within each cluster while maximizing the variance between clusters. The algorithm follows these steps:

    Initialization:
        Select k initial cluster centroids randomly from the data points.

    Assignment:
        Assign each data point to the nearest centroid, forming k clusters.

    Update:
        Recalculate the centroids of the clusters based on the mean of the data points assigned to each cluster.

    Iteration:
        Repeat the assignment and update steps until the centroids no longer change significantly or a predefined number of iterations is reached.

    Termination:
        The algorithm stops when convergence is achieved, meaning the centroids have stabilized and the clusters no longer change.

## Elbow Method

To determine the optimal number of clusters k, the Elbow Method is employed. This method involves plotting the sum of squared distances (inertia) between data points and their respective centroids against different values of k. The "elbow" point, where the rate of decrease sharply slows down, indicates the optimal number of clusters.
Project Implementation
Data Preparation

    Load and Explore the Data:
        The dataset is loaded and explored to understand its structure, statistical properties, and distribution of features.

    Handle Missing Values:
        Missing values in the categorical feature 'Gender' are imputed with the most frequent value, and 'Gender' is mapped to numerical values (0 for Male, 1 for Female).

    Feature Scaling:
        The features are standardized using StandardScaler to ensure that all features contribute equally to the clustering process.

## Clustering Process

    Optimal Number of Clusters:
        The Elbow Method is used to find the optimal number of clusters by plotting the inertia for different values of k.

    Fit K-means Model:
        The K-means algorithm is applied with the chosen number of clusters, and the resulting cluster labels are added to the dataset.

    Dimensionality Reduction and Visualization:
        Principal Component Analysis (PCA) is used to reduce the dimensionality of the data to 2D for visualization. Clusters are visualized in this reduced space to assess the clustering result.

    Evaluation:
        The silhouette score is computed to evaluate the quality of the clustering. This metric measures how similar each data point is to points in its own cluster compared to points in other clusters.

# Results and Insights

    Cluster Visualization:
        Clusters are visualized in 2D PCA space to provide an intuitive understanding of the customer segments.

    Cluster Analysis:
        The average feature values for each cluster are calculated and visualized to understand the characteristics of each customer segment.

# Contact

For any questions or further information, please feel free to reach out:

    Email: reemahmedm501@gmail.com


# Contributing

Feel free to open an issue or submit a pull request if you have suggestions or improvements.
