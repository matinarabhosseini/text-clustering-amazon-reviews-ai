# Text Clustering on Amazon Food Reviews

This repository contains an Artificial Intelligence course assignment focused on unsupervised learning and text clustering.

The project analyzes Amazon Food Reviews and groups similar reviews using modern text embedding and clustering techniques.

## Overview

The main objective is to discover hidden semantic structures within customer reviews without using labeled data.

Reviews are transformed into dense sentence embeddings and clustered using multiple clustering algorithms. The resulting clusters are evaluated both quantitatively and qualitatively.

## Dataset

The project uses the Amazon Fine Food Reviews dataset.

Each review contains:

- Review text
- Summary
- User information
- Product rating
- Helpfulness statistics

Only textual information is used for clustering.

## Project Pipeline

### 1. Text Preprocessing

The following preprocessing techniques are applied:

- Lowercasing
- Stopword removal
- Punctuation removal
- Text normalization
- Lemmatization/Stemming experiments

Different preprocessing combinations are tested and compared.

### 2. Feature Extraction

Text data is converted into numerical vectors using:

- Sentence Transformers
- all-MiniLM-L6-v2 model

These embeddings capture semantic relationships between reviews.

### 3. Clustering Algorithms

The project evaluates multiple clustering methods:

#### K-Means

- Elbow Method for K selection
- Cluster centroid analysis

#### DBSCAN

- Density-based clustering
- Noise detection
- Epsilon tuning

#### Hierarchical Clustering

- Agglomerative clustering
- Dendrogram analysis

### 4. Dimensionality Reduction

High-dimensional embeddings are reduced using:

#### PCA

- Principal Component Analysis

#### Additional Method

- t-SNE or UMAP

Reduced representations are used for visualization and cluster analysis.

### 5. Evaluation

Clusters are evaluated using:

- Silhouette Score
- Homogeneity Score
- Visual inspection
- Semantic similarity analysis

## Technologies

- Python
- Jupyter Notebook
- Scikit-Learn
- Sentence Transformers
- NumPy
- Pandas
- Matplotlib
- Seaborn
- NLP

## Repository Structure

```text
.
├── CA5_final.ipynb
├── CA5_copy.ipynb
├── AI_F04_CA5.pdf
├── amazon_reviews.csv
├── nltk_data/
└── README.md
```

## Implemented Concepts

- Unsupervised Learning
- Text Clustering
- Sentence Embeddings
- K-Means
- DBSCAN
- Hierarchical Clustering
- PCA
- t-SNE / UMAP
- Cluster Evaluation
- Semantic Similarity

## Learning Outcomes

This project provides practical experience with:

- Modern NLP embeddings
- Text clustering workflows
- Dimensionality reduction
- Cluster evaluation metrics
- Unsupervised machine learning
- Large-scale text analysis

## Academic Context

This project was developed as part of an Artificial Intelligence course assignment.

The assignment focuses on applying clustering algorithms and dimensionality reduction techniques to Amazon customer reviews and comparing their effectiveness.
