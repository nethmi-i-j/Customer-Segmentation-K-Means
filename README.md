# Customer-Segmentation-K-Means
Mall customer segmentation using K-Means clutering.

This project applies K-Means Clustering to segment mall customers based on their Annual Income and Spending Score. The goal is to identify distinct customer groups so businesses can design targeted marketing strategies, offers and discounts for each segment.

## Dataset

The dataset used is Mall_Customers.csv from Kaggle, which contains the following features:

* CustomerID
* Gender
* Age
* Annual Income (k$)
* Spending Score (1–100)

## Project Workflow

### Data Collection & Analysis

* Loaded the dataset and explored its structure (shape, info, describe)
Checked for missing values

### Feature Selection

* Selected Annual Income and Spending Score as clustering features

### Finding Optimal Clusters (Elbow Method)

* Computed WCSS (Within Cluster Sum of Squares) for cluster counts 1–10

* Plotted the Elbow Graph to determine the optimal number of clusters

* Optimal clusters identified: k = 5

### Model Building

Applied KMeans(n_clusters=5, init='k-means++')

Predicted cluster labels for each customer

### Visualization

Plotted the 5 customer segments with centroids on a scatter plot

### Results

**Key Insights**

* Red (High Income, High Spending): Most valuable customers — give them premium/loyalty offers to retain them.

* Violet (High Income, Low Spending): High potential — target with personalized offers to encourage higher spending.

* Yellow (Low Income, High Spending): Loyal despite low income — reward with  loyalty discounts to keep them engaged.

* Green (Average Income, Average Spending): Regular customers, Offer seasonal discounts and promotions to keep engage them.

* Blue (Low Income, Low Spending): Least profitable — low marketing priority.

