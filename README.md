# UnsupervisedLearning-Project6.0-LHL-

## Project Motivation and Goals
The goal of this project for me was to put the use of supervised learning techniques into practice.

## Repository folder guide/order
1. Readme
2. Unsupervised Learning Project.ipynb
3. Wholesale_Data.csv (raw data)
   
## Process

![image](https://github.com/Zarmeena667/UnsupervisedLearning-Project6.0-LHL-/assets/145514413/31f210aa-49b5-4c7f-b17e-c97dfe001d0d)



## Results/Insights
* The silhouette scores for both hierarchical clustering (0.291) and K-means (0.286) are quite close, indicating that both algorithms chosen are performing similarly in terms of cluster cohesion and separation.
* Neither score is particularly high, which suggests that there may not be very distinct clusters within my data, or that both algorithms are struggling to find a clear structure given the number of clusters specified.
* Each row in the wholesale dataframe appears to have been assigned to a cluster by each method. Both clusters have identified similar patterns however, there are rows where the two methods disagree.
* I then performed PCA using no components and plotted a graph showing the cumulative variance as a function of PCA. When using PCA for dimensionality reduction before clustering, this graph helped determine how many dimensions to retain to capture most of the information in the data. The graph plateaus around 6 and so I used 6 number of clusters. the silhouette score went up to 0.66, a clear improvement from 0.29. 
* The cluster visualization is helpful in deciphering how well the clusters formed by a clustering algorithm (like K-means or hierarchical clustering) are separated in the reduced space of the principal components. The colours represent different clusters. Ideally, we would want to see well-defined, non-overlapping clusters that indicate the algorithm has found distinct groups in the data. Some clusters seem to be well-separated while others are closer together, which might indicate some degree of similarity between those clusters. 

## Challenges
With more time, I would want to try other pre-processing techniques as well.

## Future Goals
Test further iterations of feature engineering process and use pipelines instead of code repetition. 
