# Project Title: CryptoClustering

# Description: 

Unsupervised Learning Crypto Prediction w/PCA 

# Scope: 

Using KMeans clustering w/Elbow method for K optimization to visually evaluate the effect of using PCA dimensionality reduction method on crypto currency data predictions.

View Data: [csv source](https://github.com/Ahmadhha/CryptoClustering/blob/main/Resources/crypto_market_data.csv)

View code: [jupyter notebook](https://github.com/Ahmadhha/CryptoClustering/blob/main/Crypto_Clustering.ipynb)

# Conclusions:

## 1. Best value for K without PCA optimization is 4.

![elbow_curve.](https://github.com/Ahmadhha/CryptoClustering/blob/main/Output_plots/elbow_curve.png)

## 2. KMeans cluster for scaled 7d vs 24h data:

![crypto_clusters.](https://github.com/Ahmadhha/CryptoClustering/blob/main/Output_plots/clusters.png)

## 3. Total explained variance using three principal PCA components is 89.5%.
[PC1: 0.3719856 | PC2: 0.34700813 | PC3: 0.17603793]

## 4. Best value for K with PCA optimization remains at 4 with no change.

![comp_elbow](https://github.com/Ahmadhha/CryptoClustering/blob/main/Output_plots/comp_elbow_curve.png)

## 5. Visually, it does appear that using fewer feature via PCA method slightly improved the clusters.

Notably, the yellow single point (cluster 2 in both plots) is now visually separate from the other two large clusters compared to the non-reduced plot.

However, this comparison is not sufficient to draw a conclusion, since we are only comparing it to the 7d vs 24h data, while PC1 and PC2 actually contain the majority of the reduced information. Further analysis might be required to draw a more prudent conclusion on the merit of using PCA to reduce the features for improved clustering of this dataset.

![comp_clusters](https://github.com/Ahmadhha/CryptoClustering/blob/main/Output_plots/comp_clusters.png)


