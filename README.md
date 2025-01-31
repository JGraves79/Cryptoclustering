# Cryptoclustering
Module-19
# Cryptocurrency Clustering Analysis

This project aims to cluster cryptocurrencies based on their price change percentages using K-Means clustering and Principal Component Analysis (PCA) for dimensionality reduction.

## Overview

The analysis involves the following steps:
1. **Data Loading and Preprocessing:** Import cryptocurrency market data and normalize it using `StandardScaler`.
2. **K-Means Clustering:** Determine the optimal number of clusters using the Elbow method and cluster the cryptocurrencies.
3. **Principal Component Analysis (PCA):** Reduce the dimensionality of the data to three principal components and find the optimal number of clusters using the PCA-transformed data.
4. **Visualization:** Visualize the clusters and compare the results with and without PCA.

## Libraries and Dependencies

- `pandas`
- `hvplot.pandas`
- `scikit-learn`

## Data Preparation

- Load the data from the CSV file in the Resources folder.
- Normalize the data using `StandardScaler`.
- Create a DataFrame with the scaled data.

## Finding the Optimal Number of Clusters

- Use the Elbow method to determine the best value for `k` using both the original scaled data and the PCA-transformed data.

## Clustering

- Cluster the cryptocurrencies using K-Means with the optimal `k` value.
- Compare the clustering results with and without PCA.

## Visualization

- Create scatter plots to visualize the clusters.
- Contrast the Elbow curves and clustering results.

## Key Insights

- The optimal number of clusters (`k`) for both the original and PCA-transformed data is 4.
- Using fewer features (PCA) helps to achieve tighter clustering, but more features can help classify outliers more accurately.

## How to Run the Code

1. Ensure the required libraries are installed:
   ```bash
   pip install pandas hvplot scikit-learn
