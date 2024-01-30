In this unsupervised learning assignment we will try to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.
For this we loaded this css file  crypto_market_data.csv into a DataFrame.
We renamed the file name.

Analysis file is located at Unsupervised-learning-challange-19/Crypto_Clustering.ipynb.

Preparing the DATA
Used the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
Created a DataFrame with index "coin_id".

Finding best Value for K 
Created a list from 1 to 11. then we create a for loop to compute the inertia with each possible value of k
Ploted a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

Cluster Cryptocurrencies with K-means Using the Original Scaled Data
Initialized the K-means model with the best value for k.then we Fit the K-means model using the original scaled DataFrame.
Create a scatter plot using hvPlot.

Finding the Best Value for k Using the PCA Data
Again created list, run for loop. 
Created a dictionary with the data to plot the Elbow curve.
Ploted a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

Cluster Cryptocurrencies with K-means Using the PCA Data
Initialized the K-means model with the best value for k.
Fit the K-means model using the PCA data.
Create a scatter plot using hvPlot.

Visualize and Compare
Created a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original data with the one that you created from the PCA data.
Created a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data.