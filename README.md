# Nippon Data Analysis 
# Import Libraries: 
- Import necessary libraries including pandas, numpy, seaborn, sklearn's KMeans, and matplotlib.
- Read Data: Load the dataset using pd.read_csv().
# Data Cleaning:
- Convert numeric columns from strings to floats, removing commas.
- Set the index of the DataFrame to the 'SYMBOL' column.
# Determining Optimal K:
- Compute the Within-Cluster-Sum-of-Squares (WCSS) for different values of K (number of clusters) using KMeans and store it in a list.
# Visualizing Elbow Plot:
- Plot the number of clusters against the WCSS to identify the optimal number of clusters.
# Model Fitting:
- Instantiate a KMeans model with the optimal number of clusters determined from the elbow plot.
- Fit the model to the dataset.
# Assigning Clusters: Predict the clusters for each data point in the dataset.
# Analyzing Clusters:
- Add the cluster labels to the DataFrame.
- Count the number of data points in each cluster using .value_counts()
# Output: 
- Display the DataFrame with the assigned clusters
