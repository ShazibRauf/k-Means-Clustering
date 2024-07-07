# k-Means Clustering Algorithm

This repository provides implementations of the k-Means clustering algorithm from scratch in Python. We explore different initialization strategies and compare the results on synthetic datasets.

## 1. Implementation of k-Means Algorithm

The k-Means algorithm has been implemented in Python, following the structure similar to Scikit-Learn. The implementation includes methods for fitting the clusters and predicting cluster labels for new data points.

### Methods Implemented in `K_Means` Class

#### `fit(X)`
- Runs the k-Means algorithm on the dataset `X`, assigning points to clusters and computing centroids.
- Uses either random initialization or k-means++ initialization for centroids.
- Iteratively updates centroids until convergence or after a maximum number of iterations (`max_iter`).

#### `predict(X)`
- Assigns each data point in `X` to the nearest cluster centroid based on Euclidean distance.

### Parameters

- `k`: Number of clusters to find.
- `initial_centroids`: Initial centroids for clusters, either `'random'` or `'Kmeans++'`.
- `max_iter`: Maximum number of iterations for the `fit` method.

### Required Libraries

Install the necessary Python libraries:

```bash
pip install numpy matplotlib scikit-learn
```

### Usage

Run the following command:

```bash
python kmeans-clustering.ipynb
```
