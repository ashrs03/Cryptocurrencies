# Cryptocurrencies

## Purpose 

A prominent investment bank, wants to offer new cryptocurrency investment portfolio for its customers. However, due to vast number of cryptocurrencies, they need a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. This data needs to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board. 

## Results 

As part of the analysis preprocessing of the data was the first step. THis involved following specific steps such as keeping cryptocurrencies being traded, dropping columns not required, filter the dataFrame so that it has rows where coins have been mined, creating DataFrame that holds only the cryptocurrency names, and use of the crypto_df DataFrame index as the index for this new DataFrame.Once the dataframe was created StandardScaler fit-transform function to standardize the features was used. 

Initial data frame 

![image](https://user-images.githubusercontent.com/42523379/215248542-f5bcc7fd-ccbb-4175-bb0c-3e1373ec0b60.png)

After removing rows with atleast one null value 

![image](https://user-images.githubusercontent.com/42523379/215248571-72a5c296-8147-4388-aa9a-d2a0b65afe62.png)

Data when only rows where coins are mined are kept

![image](https://user-images.githubusercontent.com/42523379/215248592-2a6f8810-d256-4dfa-9b7a-1868b3e56362.png)

Using the Principal Component Analysis (PCA) algorithm, dimensions of the X DataFrame are reduced to three principal components and these dimensions are placed in a new DataFrame.

![image](https://user-images.githubusercontent.com/42523379/215248701-a313e70f-4d10-4f4e-959c-679c321aa4fc.png)

Clustering of cryptocurrencies was performed using k-means 

![image](https://user-images.githubusercontent.com/42523379/215248743-9f2fb569-7a7b-422b-98d9-ef0a99df63a1.png)

A new dataFrame was created including predicted clusters and cryptocurrencies features.

Clusters are then plotted using a 3D scatter plot, and each data point shows the CoinName and Algorithm

![image](https://user-images.githubusercontent.com/42523379/215248858-0b9a2854-1730-4c1d-8d3e-f0d03f06dd66.png)

A table with tradable cryptocurrencies is created using the hvplot function and scstter plot is created 

![image](https://user-images.githubusercontent.com/42523379/215248928-a01a1013-b483-41be-89b6-1776ca5839f8.png)

## Summary Statement 

Unsupervised machine learning can be successfully used to group the cryptocurrencies using clustering algorithm. 
