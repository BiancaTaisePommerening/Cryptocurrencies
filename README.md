# Cryptocurrencies
Unsupervised Machine Learning

## Project Overview


## Design Solution

Preprocessing the data por PCA
    - Read the dataset into a dataframe using pandas.
    - Get the count of fows for each column in the dataframe.
    - Check the datatypes of the columns
    - Check for duplicate entries
    - Set the column that has the abbreviated name of the coins as the new index.
    - Filter the dataframe to keep only the cryptocurrencies that are being traded.
    - Filter the dataframe to keep only the cryptocurrencies that have a working algorithm.
    - Drop the column that checks if the cryptocurrencies are being traded.
    - Check null values 
    - Drop the rows that have at least one null value.
    - Check null values again
    - Check row counts
    - Keep the rows where the coins are mined, by filtering the "TotalCoinsMined" Column for vlues greater than 0.
    - Check the rows count.
    - 

Reducing Data Dimensions Using PCA

Clustering Cryptocurrencies Using K-means

Visualizing Cryptocurrencies Results



### Results



### Principal Components


![components](./Resources/components.png)

The dataframe above shows the three principal components (PCAs) generated, where data is aggregated together by the similarity of the features.

Threee PCAs were calculated 

### Elbow Curve Plot

Defining the k value on a range from 1 to 10, then using the K-mean algorithm to iterate through the k value, find their inertia and store it into a dataframe, that can then be used to generate the elbow curve plot shown below.

![elbow_curve](./Resources/elbow_curve.png)

After analyzing the elbow curve, it can be seen that the angle at point 4 looks like an elbow, which means using 4 clusters for the analysis is a good option.

### 3D Plot

![3D_plot](./Resources/3D_plot.png)

The above 3D Plot takes in 3 axis; x, y, and z corresponding the three PCAs previously calculated. This plot confirms that diving the groups into four cluster makes sense, where we can see that there are four distinct groups that correspond to the four clusters that we expected the model to break the data into.  


### Scatter Plot
![scatter_plot](./Resources/scatter_plot.png)

The scatter plot above is generated without the PCA values and that is why it is harder to see the four distinct clusters, in other words since we cannot see the depth of the points it is hard to tell if they were ideally grouped.








### Summary



-------------------------------------------------------------------------------------------------------------------------------------------

Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what you are looking for, she has decided to use unsupervised learning. To group the cryptocurrencies use the clustering algorithm. Using data visualizations to share the findings with the board.

