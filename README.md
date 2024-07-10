# Customer-Segmentation using Unsupervised Learning ( K - means )

## Problem Statement
The goal of this project is to develop a machine learning model capable of identifying and grouping customers based on their shopping patterns and behaviors. By leveraging customer data such as age, gender, annual income, and spending score, the model will segment customers into distinct groups. This segmentation will empower mall owners to:

1. Enhance Targeted Marketing: Tailor marketing efforts to specific customer groups, leading to more effective promotions and campaigns.

2. Improve Customer Experience: Personalize services and offers to meet the unique needs and preferences of different customer segments.

3. Optimize Business Operations: Streamline operations and resource allocation based on the characteristics and behaviors of various customer groups.

This project will provide actionable insights that can help mall owners boost customer satisfaction and drive business growth.

## Overview
This project aims to segment customers based on their purchasing behavior and demographics. Customer segmentation allows businesses to tailor their marketing efforts to specific groups of customers, leading to more effective marketing strategies and improved customer satisfaction. The analysis is performed using a dataset of mall customers, focusing on identifying distinct groups within the customer base.

## Dataset
The dataset used in this project is Mall_Customers.csv, which contains information about customers including their:

1. CustomerID: Unique identifier for each customer.

2. Gender: Gender of the customer.

3. Age: Age of the customer.

4. Annual Income (k$): Annual income of the customer in thousands of dollars.

5. Spending Score (1-100): A score assigned by the mall based on customer behavior and spending nature.

## Libraries used 
1. pandas - For data manipulation and analysis.

2. numpy - For mathematical calculations

3. matplotlib - For creating visualizations

4. seaborn - For creating statistical graphics

5. scikit - learn - For machine learning algorithms and preprocessing
                 Modules used:
                 a. StandardScaler for feature scaling.
                 b. KMeans for clustering.
                 c. PCA for dimensionality reduction.
                 d. silhouette_score and davies_bouldin_score for evaluating clustering performance.

## Project Structure

### 1.Data Loading and Initial Inspection: 
Load the dataset and displayed the first few rows to understand its structure.

### 2. Exploratory Data Analysis (EDA):
Examined the dataset's shape, data types, and basic statistics.
Performed univariate and bivariate analysis on the distribution of age, annual income and spending score and using histograms and box plots.
![image](https://github.com/khushiisingh11/Customer-Segmentation/assets/141178181/7d6a1504-99f1-4868-9a61-54143d13caa0)


### 3. Data Preprocessing:
There is no missing values in this dataset.
Standardized the data to ensure all features contribute equally to the clustering algorithm.
Visualized the correlation heatmap.

### 4. Feature Engineering: 
Created and analyzed new features. Visualized the correlation heatmap with new features. Then prepared these for the clustering and then performed Dimensionality Reduction using Principal Component Analysis (PCA) to reduce the dimensionality of the dataset for better visualization and performance.

### 5. Segmentation:
Applied the K-Means clustering algorithm to segment the customers.
Determinined the optimal number of clusters using the elbow method, silhouette score, and Davies-Bouldin score.
Fitting the K-Means model and predict the clusters for each customer.

### 6. Visualization:
Visualizing the clusters to interpret the results and gain insights.
Using scatter plots and 3D plots to display the clusters based on grouping customers based on their purchasing behavior and demographics to target marketing strategies effectively.


### Algorithm Used - 
K-Means Clustering: This unsupervised machine learning algorithm partitions the data into a predefined number of clusters. Each data point is assigned to the cluster with the nearest mean, and the algorithm iteratively refines the cluster centers to minimize the within-cluster sum of squares (WCSS).

Principal Component Analysis (PCA): This dimensionality reduction technique is used to reduce the number of features in the dataset while retaining most of the variance. This helps in better visualization and performance of the clustering algorithm.


