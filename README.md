# Overview

This project applies unsupervised machine learning techniques to analyze and cluster cryptocurrencies based on their 24-hour and 7-day price changes. Using K-Means clustering, we explore how different feature sets affect the clustering results, including the impact of Principal Component Analysis (PCA) for dimensionality reduction.

## Objectives

- Normalize cryptocurrency market data for clustering.
- Determine the optimal number of clusters (k) using the Elbow Method.
- Perform K-Means clustering on both the original and PCA-transformed datasets.
- Compare clustering results before and after PCA to assess efficiency and accuracy.
- Visualize and interpret the clustering patterns.

## Technologies Used

Python (Jupyter Notebook)
Pandas – Data manipulation and analysis
scikit-learn – K-Means clustering, StandardScaler, PCA
hvPlot – Interactive visualizations

## Methodology

1. Data Preprocessing
Load crypto_market_data.csv into a Pandas DataFrame.
Normalize the data using StandardScaler from scikit-learn.
2. Determine Optimal Clusters (k) Using the Elbow Method
Compute inertia values for k = 1 to 11.
Plot the Elbow Curve to identify the optimal number of clusters.
3. K-Means Clustering on Scaled Data
Fit a K-Means model using the best k-value found.
Visualize the clustered data using hvPlot scatter plots.
4. Optimize Clustering with Principal Component Analysis (PCA)
Reduce dimensionality to three principal components (PC1, PC2, PC3).
Compute the explained variance ratio of PCA.
Apply K-Means clustering on the PCA-transformed data.
Compare the new clustering results with those from the original dataset.
5. Visualization & Interpretation
Scatter plots of clusters before and after PCA.
Insights on how reducing features with PCA affects clustering performance.
Key Findings

Using PCA simplified the dataset without losing meaningful patterns.
The Elbow Method helped determine an optimal k-value, ensuring better-defined clusters.
Clusters became more distinct and interpretable after applying PCA.
Results & Visualizations

## Conclusion

This project demonstrates how unsupervised machine learning can be used to analyze cryptocurrency price movements. Applying PCA enhances clustering efficiency while preserving accuracy, making it a valuable technique for handling high-dimensional financial data.
