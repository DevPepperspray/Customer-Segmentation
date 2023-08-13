# Customer-Segmentation
An Algorithm was created to Cluster customers of a mall based on their Income and Spending scores



This was an unsupervised learning project to understand the target customers for the marketing team to plan a strategy and divide the mall market targets into groups.

I downloaded the Mall Customer Datast from https://absentdata.com/data-analysis/where-to-find-data/ and then parsed the CSV file into a data frame using the Pandas Library.

I performed a quick EDA (Exploratory Data Analysis) on the dataset creating a loop to iterate through the columns we are interested in ( Age, Annual Income, and Spending Score) to create a visualization for each of them ( boxplots and histograms). Also further using the Gender column/data as a hue to further drill the data.

I plotted/visualized using a scatter chart of Annual Income against Spending score to observe the Clusters, also visualizing the correlation between Age, Spending Socre, and Annual Income using a Heatmap.


**Univariate Clustering (Income Clusters)**


Using the K-means Clustering Algorithm, I fit the annual income columns/data into the algorithm to create clusters that the customers will fall into, using the data to train the algorithm. I used the Inertia method which measures how well a dataset was clustered by K-Means. It is calculated by measuring the distance between each data point and its centroid, squaring this distance, and summing these squares across one cluster. 
From the inertia method, I derived the best-suited number of clusters to use for my income cluster algorithm. The customers were divided into clusters using the Data. I saved and appended the output to the existing data frame.

**Bivariate Clustering (Income and Spending CLsuters)**

Using the Kmeans clustering algorithm, I fit the Annual income and Spending score columns/data into the algorithm to create clusters which the customers will fall into, using the data to train the algorithm. I used the Inertia method to get the best-suited number of Clusters to use and edited my algorithm and appended my data frame with the output.

Add-ons: Created a Centroid in the visualization indicated with the *(star) symbol for easy interpretation.

**Summary statistics on the clusters**


The target group would be cluster 0, which has a high spending score and high income. There should be a reach-out/ campaign/ discount for these customers to encourage and entice these customers to ensure continuous patronizing.

Cluster 4 represents an interesting opportunity for future major customers as they are the youngest customers but have high spending scores(probably purchasing one-off gadgets like PS4 and designer products like Jordans.

Lastly, Cluster 3. These are customers with high Annual income but low spending scores. Surveys should be carried out on how best their needs can be met as they have the necessary purchasing power.

I saved the new Dataframe as a CSV (Customer ID, Age, Annual Income, Spending Score, Income Cluster, Income, and Spending Cluster).



