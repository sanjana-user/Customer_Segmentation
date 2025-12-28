# Customer_Segmentation

# **Problem Statement:** 

Understanding customer behavior helps in targeted marketing and providing personalized services. The goal of this project is to segment customers into different groups based on their purchasing behavior and demographics using unsupervised learning techniques. 

# **Dataset:**

The dataset is taken from Kaggle, consisting of customer demographic and purchasing behavior data, including age, annual income, and spending score. It is used for unsupervised learning to identify distinct customer segments.

## **Rows:** 200

## **Features:** Age, Annual Income, Spending Score.

## **Target Variable:** None (unsupervised)

# **Tools:**

Pandas

Numpy 

Matplotlib

Seaborn 

Scikit Learn

# **Approach and Methodology:** 

- Cleaned the Data
- 
## **Data Visualisation:**
  
- Visualised the data considering Annual Income, Age and Spending Score of the customers individually.
  
- Observed the scatter plots for every two variables using pairplot.
  
- Visualised the correlation matrix of all the features by converting them to numerical data.
  
## **Univariate:**

-A K means model is created with one feature, Annual Income. (most correlation), by taking the k values in the range 1-10, and checking WCSS scores for each value of k.

- Now plotting the elbow plot (WCSS scores vs k values), gave us the k value for our case.
  
## **Bivariate:**

- Similarly, the features Annual Income and Spending Scores are considered to compute the k value.
   
- The scatter plot can be visualised directly, by grouping the values by their clustering labels.
  
## **Multivariate:**

- Similarly tried for k value in the range 1-10 realising there’s no elbow plot.
  
- Modifying the range to be 1-30 gave us the k value to be 13 (beyond 10).
 
# **Models used:**

**K Means Clustering:** It's used to group unlabeled data into a predefined number of clusters, denoted by K. It's done using elbow plot, where the WCSS are plotted against k values in a range. 

# **Evaluation Metrics:**

## **Inertia scores or WCSS (Within cluster sum of squares):** 
It calculates the sum of squared distances between each data point and the centroid of its assigned cluster. As the number of clusters increases, WCSS typically decreases because data points are grouped into smaller, more specific clusters, but the rate of decrease slows down after a certain point, forming an "elbow" shape when plotted against the number of clusters.

## **Clustering Labels:** 

- Labels are assigned to each cluster component from 0 to (k-1).

- They can be made a new column grouping by which the scatter plots can be visualised.

# **Insights:**

- Customers were grouped into distinct segments based on income and spending behavior.
  
- Univariate (Annual Income) had 3 clusters.
  
- Bivariate (Annual Income and Spending Scores) had 5 clusters and multivariate 13.
   
# **How to run the project:**

- Download or clone the repository.
  
- Open the project folder.
  
- Open the Jupyter Notebook file (.ipynb).
  
- Run all the cells from top to bottom.

# **Project Structure:**

├── Mall_Customers.csv        # Dataset used in the project

├── Customer.Segmentation.ipynb      # Jupyter Notebook with full code

├── README.md          # Project explanation
