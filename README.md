# Clustering Analysis on Wine Dataset

## Overview
This lab focuses on applying unsupervised clustering techniques to the Wine Dataset from the `sklearn.datasets` library. Two clustering algorithms, K-Means and K-Medoids, were implemented to identify natural groupings within the data. The performance of each algorithm was evaluated using the Silhouette Score and Adjusted Rand Index (ARI), and the results were visualized using Principal Component Analysis (PCA).

## Objectives
- Implement both K-Means and K-Medoids clustering algorithms.  
- Evaluate clustering performance using Silhouette Score and Adjusted Rand Index.  
- Visualize and interpret cluster separations using PCA-reduced data.  
- Compare both approaches and understand when each is most effective.

## Results Summary
The K-Means algorithm achieved a Silhouette Score of 0.285 and an Adjusted Rand Index of 0.897.  
The K-Medoids algorithm produced a Silhouette Score of 0.266 and an Adjusted Rand Index of 0.726.  

K-Means generated more compact and accurate clusters that closely matched the actual wine classes.  
K-Medoids formed slightly less cohesive clusters but demonstrated better robustness to potential outliers.


## Insights
The Wine dataset consists of 13 standardized numerical features representing different chemical properties of wines from three cultivars. After normalization, K-Means performed better because the dataset is clean, continuous, and well-suited for centroid-based clustering. K-Medoids, while less precise in this context, is more stable when datasets contain outliers or non-spherical distributions.  

Both algorithms successfully revealed three main groupings that correspond to the true wine categories, confirming that clustering effectively captures the underlying data structure.


## Challenges
A few challenges were encountered during the lab:
- Proper standardization was essential to prevent scale differences from biasing distance calculations.  
- Visualizing 13-dimensional data in two dimensions required PCA, which can slightly distort true spatial relationships.  
- Understanding how centroids (K-Means) differ from medoids (K-Medoids) helped in interpreting the results correctly.



## Conclusion
This lab demonstrated how clustering algorithms can uncover hidden patterns in multidimensional data.  
The K-Means method performed better on this dataset, forming more compact and accurate clusters.  
The K-Medoids method, while less precise, remains a valuable alternative when working with datasets containing noise or irregular cluster shapes.  
Overall, this experiment highlighted the importance of data preprocessing, metric-based evaluation, and visualization in effective clustering analysis.
