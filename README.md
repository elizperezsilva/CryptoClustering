# CryptoClustering
Module 19 Challenge - Elizabeth Perez Silva

# Background
Using knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

# Instructions from Canvas

## Prepare the Data
- Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
- Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

## Find the Best Value for k Using the Scaled DataFrame
Use the elbow method to find the best value for k using the following steps:
- Create a list with the number of k values from 1 to 11.
- Create an empty list to store the inertia values.
- Create a for loop to compute the inertia with each possible value of k.
- Create a dictionary with the data to plot the elbow curve.
- Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
- Answer the following question in your notebook: What is the best value for k?

## Cluster Cryptocurrencies with K-means Using the Scaled DataFrame
Use the following steps to cluster the cryptocurrencies for the best value for k on the scaled DataFrame:
- Initialize the K-means model with the best value for k.
- Fit the K-means model using the scaled DataFrame.
- Predict the clusters to group the cryptocurrencies using the scaled DataFrame.
- Create a copy of the scaled DataFrame and add a new column with the predicted clusters.
- Create a scatter plot using hvPlot

## Optimize Clusters with Principal Component Analysis
- Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
- Retrieve the explained variance to determine how much information can be attributed to each principal component
- Create a new DataFrame with the scaled PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

## Find the Best Value for k Using the PCA DataFrame
Use the elbow method on the scaled PCA DataFrame to find the best value for k using the following steps:
- Create a list with the number of k-values from 1 to 11.
- Create an empty list to store the inertia values.
- Create a for loop to compute the inertia with each possible value of k.
- Create a dictionary with the data to plot the Elbow curve.
- Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

## Cluster Cryptocurrencies with K-means Using the PCA DataFrame
Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA DataFrame:
- Initialize the K-means model with the best value for k.
- Fit the K-means model using the scaled PCA DataFrame.
- Predict the clusters to group the cryptocurrencies using the scaled PCA DataFrame.
- Create a copy of the scaled PCA DataFrame and add a new column to store the predicted clusters.
- Create a scatter plot using hvPlot
  
# Code Source
- Module 19 exercises and solutions from class
- Lectures from week 19 on zoom recordings
- Further reading resources in Module 19 
