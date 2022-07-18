# Cryptocurrencies

## Overview

The purpose of this project is create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. The initial data that we are working with is not idea, so it will need to be cleaned and processed to fit the machine learning models. Because there is no known output for what I am looking for, I've decided to use unsupervised machine learning, and clustering algorithms to create data visualizations to share my findings.

## Results 

### StandardScaler
Using StandardScaler, we standardize the features as well as ensure that:
- All cryptocurrencies that are not being traded are removed
- The IsTrading column is dropped 
- All the rows that have at least one null value are removed 
- All the rows that do not have coins being mined are removed
- The CoinName column is dropped 
 
![StandardScaler](https://user-images.githubusercontent.com/98790082/179435616-06885b6d-4a77-400f-9337-bd09d699e66d.png)


### Principal Component Analysis
Using the Principal Component Analysis (PCA) algorithm, you’ll reduce the dimensions of the DataFrame to three principal components

![PCA](https://user-images.githubusercontent.com/98790082/179435890-a45e826d-f01e-4dd5-b020-1170b5f74aac.png)

### K-means Algorithm
create an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame and run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.

![PredictedCluster](https://user-images.githubusercontent.com/98790082/179435979-21c1aaf8-6b0b-42ff-a11a-9399f30faff2.png)

### Plotly Express
By creating scatter plots with Plotly Express and hvplot, we'll visualize the distinct groups that correspond to the three principal components we created
![CoinSupplyvsCoinMined](https://user-images.githubusercontent.com/98790082/179436127-d15a19c3-3877-4c43-81f2-9ccad39bac14.png)

![ElbowCurve](https://user-images.githubusercontent.com/98790082/179436222-9f3b4908-8cdd-4730-bc7c-99a54a1b11c7.png)

![3DClusterWithScatters](https://user-images.githubusercontent.com/98790082/179436229-97b7b51e-4e22-4d8e-83f4-f597d5cd4574.png)
