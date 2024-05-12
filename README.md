# CryptoClustering

# CryptoClustering Project

## Overview
This project aims to classify cryptocurrencies according to their price fluctuations over various time frames using the K-means clustering algorithm and Principal Component Analysis (PCA). The analysis spans intervals of 24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year to gain insights into how different cryptocurrencies behave financially.


## Data Preparation
- **Normalize the Data**: Utilize `StandardScaler` from scikit-learn to normalize the dataset.
- **Create Scaled DataFrame**: Ensure the `coin_id` from the original DataFrame remains as the index in the new scaled DataFrame.

## Finding the Best Value for k
- **Elbow Method**: Implement the elbow method by iterating from 1 to 11 clusters to determine the optimal `k` value.
- **Inertia Calculation**: Store and plot inertia values to visually identify the best value for `k`.

## Clustering Cryptocurrencies
- **K-Means Clustering**: Use K-Means to cluster data based on the best value for `k` determined from the scaled and PCA-transformed data.
- **Analysis of Clusters**: Analyze and visualize the clustering results to interpret market behaviors.

## Principal Component Analysis (PCA)
- **Dimensionality Reduction**: Reduce features to three principal components and analyze the explained variance.
- **Cluster Optimization**: Reapply the elbow method using PCA data to refine cluster assignments.

## Results and Visualization
- Create scatter plots to visualize clusters based on price changes and principal components.
- Determine which features heavily influence the principal components.

## Technologies Used
- Python: Primary programming language.
- Pandas and NumPy: For data manipulation.
- Scikit-learn: For implementing PCA and K-Means clustering.
- hvPlot and Matplotlib: For data visualization.
- Jupyter Notebook: For executing and sharing the project workflow.
---

