# Cryptocurrencies and Unsupervised Machine Learning


## Project Overview

The motivation behind this project is to utilize unsupervised machine learning to analyze cryptocurrency data. The original dataset came from CryptoCompare and can be seen in the raw format [here](https://min-api.cryptocompare.com/data/all/coinlist). 

Ahead of creating the data visualizations, the cryptocurrency file was preprocessed using the Pandas and Scikit-learn libraries. The Principal Component Analysis (PCA) algorithm was then used to reduce the high dimensionality of the data. This set the stage for use of the K-means algorithm – which is (currently) considered one of the fastest and most efficient algorithms used to categorize data points into groups, especially when little information is available about the data.

## Resources
* Python 
* Plotly library
* Scikit-learn library
* Pandas library
* Jupyter Notebook
* Data Sources: .csv and .ipynb files

## Results

Below you will see the data visualizations that were created for this project. 

### Elbow Curve
![elbow_curve_crypto](https://github.com/Kelfang/Cryptocurrencies/blob/main/images/elbow_curve_crypto.png)

As illustrated in the elbow curve image above, the optimal number of clusters is four. This method helped us find the ideal value of k in the K-means algorithm. 

-------------------------------------------------------------
### 3-D Scatter Plot
![crypto_scatter_plot3d](https://github.com/Kelfang/Cryptocurrencies/blob/main/images/crypto_scatter_plot3d.png)

The image above uses the three principal components from the PCA algorithm and was created after implementing the K-means algorithm. In a general view of this plot, it appears there is solid cohesion within the clusters. Additionally, the separation is very apparent for the most part, except for Classes 0 and 2, which are in close proximity of one another. 

-------------------------------------------------------------
### hvPlot Table


![hvplot_table_crypto](https://github.com/Kelfang/Cryptocurrencies/blob/main/images/hvplot_table_crypto.png)

The table above lists the 532 tradable cryptocurrencies and is sortable by columns. This kind of data presentation helps bridge the gap for individuals that may be more spreadsheet oriented or want additional reference for the other visualizations shown within this project.

-------------------------------------------------------------
### hvPlot Scatter Plot
![hvplot_scatter_crypto](https://github.com/Kelfang/Cryptocurrencies/blob/main/images/hvplot_scatter_crypto.png)

Turning the focus to the Total Coins Minted and Total Coin Supply, in the image above, we can see the cryptocurrency data in a different way. 

By offering different visualizations, this increases the opportunity for everyone to benefit from the unsupervised machine learning methods. 

-------------------------------------------------------------
*To view all of the code used to create the visualizations above, please click [here]( https://github.com/Kelfang/Cryptocurrencies/blob/main/crypto_clustering.ipynb).*


