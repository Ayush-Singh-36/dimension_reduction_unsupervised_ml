Dimensionality Reduction Project: PCA vs t-SNE
Overview
This project explores the application of two popular dimensionality reduction techniques—Principal Component Analysis (PCA) and t-distributed Stochastic Neighbor Embedding (t-SNE)—on the classic Iris flower dataset. The goal is to project high-dimensional data (4 features) into a 2D space for visualization and pattern discovery.

Dataset
The Iris Dataset consists of 150 samples from three species of Iris (Iris setosa, Iris virginica, and Iris versicolor). Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters.

Methodology
1. Principal Component Analysis (PCA)
PCA is a linear dimensionality reduction technique that identifies the axes (principal components) along which the variance of the data is maximized. It is computationally efficient and great for preserving the global structure of the data.

2. t-distributed Stochastic Neighbor Embedding (t-SNE)
t-SNE is a non-linear technique particularly well-suited for the visualization of high-dimensional datasets. It works by converting similarities between data points to joint probabilities and minimizes the Kullback-Leibler divergence between the joint probabilities of the low-dimensional embedding and the high-dimensional data. It is excellent at preserving local structures and clusters.

Requirements
To run this project, you need the following Python libraries installed:

pandas
seaborn
matplotlib
scikit-learn
How to Use
Load the Iris dataset using Seaborn.
Preprocess the data by removing categorical columns (like 'species').
Apply PCA from sklearn.decomposition to reduce dimensions to 2.
Apply TSNE from sklearn.manifold to reduce dimensions to 2.
Visualize the results using scatter plots, color-coded by species to evaluate cluster separation.
