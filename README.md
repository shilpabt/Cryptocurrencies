# Cryptocurrencies
Unsupervisd machine learning is used for, how to process data, how to cluster, how toreduce dimensions and how to reduce principal components using PCA. Machine learning algorithms discover data groupings without the human intervention.

This project uses cryptocurrency data and try to categorize them to build a classifiction system for new investors. A prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. They need a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. Since there is no known output, we must decided to use unsupervised learning.

To group the cryptocurrencies, we will use clustering algorithm and will use data visualizations to share our findings with the board.

## Resources

Python
Scikit-learn 1.1.0
Plotly Express
hvPlot 
Pandas


# Results  
## Deliverable 1: Preprocessing the Data for PCA
Preprocessed dataset using Pandas, in order to perform PCA  

   Crypto data                        |  Preprocessed data
:------------------------------------:|:-------------------------:
![](images/crypto_data.png?raw=true)  |  ![](images/preprocessed_data.png?raw=true)


## Deliverable 2: Reducing Data Dimensions Using PCA   
Using your knowledge of how to apply the Principal Component Analysis (PCA) algorithm, reduced the dimensions of the X DataFrame to three principal components and placed these dimensions in a new DataFrame.

![](images/reduced_data_dimensions.png?raw=true)


## Deliverable 3: Clustering Cryptocurrencies Using K-means
Finding the Best Value for 'k' Using the Elbow Curve
![](images/Elbow_curve.png?raw=true)

Created a new DataFrame including predicted clusters and cryptocurrencies features and concatentated the crypto_df and pcs_df DataFrames on the same columns.

![](images/clustered_data.png?raw=true)

## Deliverable 4: Visualizing Cryptocurrencies Results

Created a 3D scatter plot using the Plotly Express scatter_3d() function to plot the three clusters from the clustered_df DataFrame.

![](images/3D_cluster.png?raw=true)


Using the knowledge of creating scatter plots with Plotly Express and hvplot,visualize the distinct groups that correspond to the three principal components created in Deliverable 2, then created a table with all the currently tradable cryptocurrencies using the hvplot.table() function.

![](images/tradable_cryptocurrencies.png?raw=true)

Scaled the TotalCoinSupply and TotalCoinsMined columns between the given range of zero and one using the MinMaxScaler().fit_transform method.

![](images/new_clustered_data.png?raw=true)

Created hvplot scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class", and it shows the CoinName when you hover over the the data point.

![](images/scattered_plot.png?raw=true)





