# Market Basket Analysis & Customer Segmentation

## Overview

This project performs an end-to-end Market Basket Analysis on online retail transaction data. By applying Unsupervised Machine Learning techniques, the project identifies hidden purchasing patterns and segments customer transactions into distinct clusters. These insights can be leveraged for targeted marketing, product bundling, and optimizing store layouts.

## Problem Statement

The business possesses transaction records containing multiple products purchased together but lacks a systematic analysis of these shopping baskets. The objective is to analyze the data using statistical and machine learning techniques, identify similarities between transactions, compare clustering algorithms, and derive meaningful business conclusions.

## Dataset

The dataset (`Online retail_new.csv`) contains row-by-row transaction data where each row represents a single customer's shopping basket and the columns represent the items purchased.

## Methodology

The analysis follows a structured data science pipeline:

1. **Data Preprocessing & EDA:**
* Handled the row-based dataset structure to calculate transaction sizes and item frequencies.
* Visualized the Top 10 most frequent products and the distribution of basket sizes.


2. **Feature Engineering:**
* Transformed categorical transaction data into a numerical binary matrix using One-Hot Encoding.


3. **Dimensionality Reduction:**
* Applied Principal Component Analysis (PCA) to reduce the high-dimensional product matrix into a 2D feature space for visualization and computational efficiency.


4. **Clustering & Evaluation:**
* Implemented four clustering algorithms: **K-Means**, **Hierarchical**, **DBSCAN**, and **Spectral Clustering**.
* Evaluated model performance mathematically using the **Silhouette Coefficient** and **Davies-Bouldin Index**.



## Technologies Used

* **Python 3**
* **Pandas & NumPy:** Data manipulation and matrix transformations.
* **Matplotlib & Seaborn:** Data visualization.
* **Scikit-Learn:** PCA dimensionality reduction, clustering algorithms, and evaluation metrics.

## Key Findings & Business Implications

* **Algorithm Performance:** (Add a brief note here based on your actual Colab output, e.g., "K-Means provided the most distinct clusters based on the Silhouette score.")
* **Targeted Marketing:** Identified distinct buyer profiles (e.g., bulk buyers vs. single-item shoppers), allowing for personalized email campaigns and homepage recommendations.
* **Product Bundling:** Frequently co-occurring items can be bundled together at a slight discount to increase the average order value.

## How to Run the Notebook

1. Clone this repository to your local machine.
2. Ensure you have Jupyter Notebook or Google Colab available.
3. Upload the `Online retail_new.csv` dataset to your working environment.
4. Run all cells in the `Market_Basket_Analysis.ipynb` notebook sequentially to view the data pipeline, visualizations, and model evaluations.
