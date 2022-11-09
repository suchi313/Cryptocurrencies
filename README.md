# Cryptocurrencies

## Overview 
The purpose of this analysis is to analyze a database of cryptocurrencies by utlizing unsupervised machine learning. This challenge allowed us to create a report to share the results of the widely recognized cryptocurrencies classified by group according to their features. 

## Resources 

Datasource: CryptoCompare and crypto_data.csv
Software: Python 3.10, Anaconda Navigator, Conda, Jupyter Notebook

## Results

### 3D Plot 

This 3D plot was generated from this code:

```
# Creating a 3D-Scatter with the PCA data and the clusters
fig = px.scatter_3d(
    clustered_df,
    x='PC 1',
    y='PC 2',
    z='PC 3',
    color='Class',
    symbol='Class',
    hover_name= 'CoinName',
    hover_data= ['Algorithm'],
    width=800,
)
fig.update_layout(legend=dict(x=0, y=1))
fig.show()
```



![3D Plot](https://user-images.githubusercontent.com/102767530/200730725-cc612be0-048f-4358-a585-c8a16057f7c9.png)
