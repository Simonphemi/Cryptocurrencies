# Cryptocurrencies
## Analysis_Overview
  For this project unsupervised machine learning was used to anlayze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified into clusters based on their features. This report could be used to categorize different currencies being traded in the market for further analysis.

  In order to accomplish this task, the data was processed to remove all null values, filtered for currencies only which were traded and coins which were mined. We then converted the string variables into numeric variables using the "get_dummies" function in the pandas library. After the data was processed, it was scaled using StandardScaler and data dimensions were reduced to three using PCA.
  
  <img width="646" alt="Clustered_DataFrame_W_PC1_PC2_PC3" src="https://user-images.githubusercontent.com/79813670/124412365-56cc8980-dd1c-11eb-8f0f-d8bec9905527.png">

Using the final PCA dataframe, we performed K-means clustering to categorize the data into 4 classes. We ended up at 4 clusters by utilizing the elbow curve.

<img width="815" alt="Elbow_Curve" src="https://user-images.githubusercontent.com/79813670/124412392-69df5980-dd1c-11eb-8eec-efe98b0d912f.png">

Finally we created visualizations of our machine learning results. We created a 3D scatter plot of the three PCA Dimensions (screenshot included below)

<img width="806" alt="3D_plot_Scatter_Cluster" src="https://user-images.githubusercontent.com/79813670/124412425-7a8fcf80-dd1c-11eb-9ac8-6edc134e7eb4.png">

Also a 2D Scatter plot was created by going back to our original dataset (before applying scaling using StandardScaler). We extracted the two variables coins mined and coins supply and performed a second scaling using MinMaxScaler. We then plotted the data on a 2D Scatter plot.

<img width="783" alt="hv_Scatter_Plot_W_TCM_ _TCS" src="https://user-images.githubusercontent.com/79813670/124412505-aca13180-dd1c-11eb-9652-9e8c6e96204c.png">

