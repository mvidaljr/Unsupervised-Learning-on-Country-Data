# Unsupervised Learning on Country Data


## Project Overview

This project focuses on unsupervised learning techniques to cluster countries based on various socioeconomic and health-related indicators. The goal is to identify similar groups of countries that can be used for comparative analysis and decision-making.

## Dataset

- **Source:** The dataset for this project was downloaded from Kaggle via [Unsupervised Country Data](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data/data).
- **Features:** The dataset includes various indicators such as income, child mortality, GDP, and other metrics that reflect the socioeconomic and health status of different countries.

## Tools & Libraries Used

- **Data Analysis:**
  - `Matplotlib` (Graphic plot)
  - `Groupby()`
  - `info()`
  - `duplicated()`
  - `isnull()`
  - `describe()`
- **Data Visualization:**
  - `seaborn.heatmap()` for plotting dataset correlations
- **Data Preprocessing:**
  - `sklearn MinMaxScaler` for data normalization
- **Model Training:**
  - `KMeans` for clustering countries
  - `KneeLocator` (Elbow method) to determine the optimal number of clusters (K)
  - `scipy.cluster.hierarchy` for plotting a dendrogram to visualize hierarchical clustering

## Methodology

1. **Data Exploration:**
   - Conducted exploratory data analysis (EDA) to understand the distribution and structure of the dataset.
   - Identified and handled missing values and duplicates.

2. **Feature Engineering:**
   - Visualized feature correlations using a heatmap to understand the relationships between different indicators.

3. **Data Normalization:**
   - Applied `MinMaxScaler` to normalize the data, ensuring that all features contribute equally to the clustering process.

4. **Clustering:**
   - Implemented the `KMeans` algorithm to cluster countries into distinct groups.
   - Used the `KneeLocator` (Elbow method) to determine the optimal number of clusters (K), enhancing the quality of the clustering.

   ### Elbow Method Explanation
   The Elbow Method is used to determine the optimal number of clusters (K) in a KMeans algorithm. It works by plotting the sum of squared distances (inertia) between data points and their assigned cluster centroids for different values of K. As K increases, the inertia decreases, but at some point, the rate of decrease slows down. The "elbow" point on the graph indicates the optimal K value, where adding more clusters does not significantly improve the model. This helps in selecting a K that balances complexity and performance.


5. **Hierarchical Clustering:**
   - Visualized the hierarchical relationships between clusters using a dendrogram, generated with `scipy.cluster.hierarchy`.


## Results

- Successfully identified several clusters of countries with similar socioeconomic and health characteristics.
- The optimal number of clusters was determined using the Elbow method, leading to a meaningful segmentation of the data.

## Conclusion

The project demonstrated the effectiveness of unsupervised learning techniques in clustering countries based on key indicators. These clusters can provide valuable insights for comparative analysis and policy-making.

## Future Work

- Explore more sophisticated clustering techniques such as DBSCAN or Gaussian Mixture Models.
- Investigate the impact of different feature selection methods on clustering outcomes.
- Extend the analysis to include time-series data for tracking changes in cluster membership over time.


![image](https://github.com/mvidaljr/Unsupervised-Learning-on-Country-Data/assets/103943988/18de633a-cfed-4531-91b8-7bb0baf63a8c)
