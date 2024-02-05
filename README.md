##  Module 19 Challenge
* Project Name: Crypto Clustering
* Submitted by:  Michael Jardinico
* Date Submitted: Feb 3, 2024

### Project Overview
`This project focuses on clustering cryptocurrencies based on their market data. It involves setting up a GitHub repository, organizing files, and running a Jupyter Notebook for data analysis. This README outlines the steps to set up and execute the project.`

### Working Files
1. `Crypto_Clustering.ipynb`
2. `/Resources/crypto_market_data.csv`
    
### Instructions
1. __GitHub Repository Setup:__
    - Create a Repository: Start by creating a GitHub repository named `CryptoClustering`.
    - Clone to Local: Clone the repository to your local computer using Git.

2. __File Organization:__ 
    - Download the starter files: Obtain the starter files from [Starter_Code](https://github.com/mjardinico/CryptoClustering/tree/main/Resources/Starter_Code).
    - Create a `Resources` directory and save the `crypto_market_data.csv` file in it.
    - Main Code: Use [Crypto_Clustering.ipynb](https://github.com/mjardinico/CryptoClustering/blob/main/Crypto_Clustering.ipynb) as the primary code for this project.

3. __Data Preparation__
`Import the necessary libraries and modules for data analysis:`
    - import pandas
    - import hvplot.pandas
    - from sklearn.cluster import KMeans
    - from sklearn.decomposition import PCA
    - from sklearn.preprocessing import StandardScaler
   
4. __Data Processing__  

    - __Normalize the Data:__ Use the `StandardScaler()` from `scikit-learn` to normalize the data.

    - __Create Scaled DataFrame:__ Construct a DataFrame with the scaled data, ensuring the "coin-id" is set as the index.
    ![Crypto Currency DataFrame](https://github.com/mjardinico/CryptoClustering/blob/main/Resources/crypto_dataframe1.png) 
    
    - __Elbow Curve:__ Generate an elbow curve to identify the optimal value of k. 
    ![Elbow Curve](https://github.com/mjardinico/CryptoClustering/blob/main/Resources/elbow_curve.png)

    - __Principal Component Analysis (PCA):__ Optimize clusters using PCA.
    ![PCS DataFrame](https://github.com/mjardinico/CryptoClustering/blob/main/Resources/PCA_DataFrame.png)

    - __Cluster Scatter Plot:__ Create a scatter plot using `hvplot` using `KMeans`
    ![PCA Scatter Plot](https://github.com/mjardinico/CryptoClustering/blob/main/Resources/cluster_scatterplot1.png)


`NOTE: Rendering of interactive plots on GitHub is not supported. Use Jupyter Notebook to view interactive plots correctly.`