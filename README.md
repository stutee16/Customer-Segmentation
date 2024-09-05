# Customer Segmentation for Targeted Marketing using Unsupervised Clustering

## Introduction
The project, **Customer Segmentation for Targeted Marketing using Unsupervised Clustering**, is designed to help businesses better understand their customer base by identifying unique customer segments through data-driven techniques. Using unsupervised clustering methods, we aim to group customers based on shared traits, such as spending patterns and personal attributes, allowing businesses to tailor marketing strategies and improve customer engagement. 

By leveraging clustering, businesses can optimize marketing efforts, improve customer retention, and enhance overall profitability by focusing on segment-specific needs and preferences.

## Objective
The objective of this project is to:
- Analyze customer data and group them into distinct clusters.
- Simplify complex data using **dimensionality reduction** to enhance cluster interpretation.
- Generate meaningful insights to assist in **targeted marketing strategies**.
- Develop detailed customer profiles for each segment to identify high-value customers and those who need more attention.

## Data Preprocessing
Before diving into the analysis, the data underwent various preprocessing steps:
- **Data Cleaning**: Removing any missing, duplicated, or irrelevant data.
- **Feature Engineering**: Creating new features such as `Age`, `Spent`, `Living_With`, `Children`, `Family_Size`, and `Is_Parent` to enhance analysis.
- **Handling Categorical Data**: Transforming categorical variables into meaningful numeric representations using techniques like one-hot encoding and label encoding.
- **Scaling**: Normalizing or standardizing features to ensure uniformity in data.

## Dimensionality Reduction
To handle the large number of features in the dataset, we applied **Principal Component Analysis (PCA)** for dimensionality reduction. PCA helps simplify the data by capturing the most important features while minimizing information loss. For this project, we reduced the data to three principal components to ensure that clustering remains effective without over-complicating the model.

## Clustering
### Agglomerative Clustering
Once dimensionality reduction was completed, **Agglomerative Clustering** was used to group customers. This hierarchical clustering method begins by treating each customer as its own cluster and merges them iteratively based on similarity, forming larger clusters until the desired number is achieved. 

### Steps in Clustering:
- **Elbow Method**: Used to determine the optimal number of clusters.
- **Agglomerative Clustering**: Performed on the reduced data to create the final customer segments.
- **Cluster Visualization**: Examined using 2D and 3D scatter plots to visualize how the data has been grouped.

## Profiling
After clustering, detailed customer profiles were created for each cluster. These profiles allowed for the examination of:
- **Spending Habits**: Identifying the products (Wines, Fruits, Meat, Fish, Sweets, Gold) that each cluster spends the most on.
- **Demographics**: Age, family size, and parenthood status, which helped determine the personal characteristics of each segment.
- **Income & Spending**: Analyzing the spending patterns in relation to income levels for each cluster.

## Results
The segmentation revealed insightful differences among the clusters:
- **Cluster 0**: High spending with average income. They are mostly parents and have families of 2-4 members, with teenagers in the household.
- **Cluster 1**: High spending with high income. They do not have children and tend to be couples or singles, spanning all age ranges.
- **Cluster 2**: Low spending with low income. They are relatively younger and tend to have small families with one child.
- **Cluster 3**: High spending with low income. This group is also made up of parents, with 2-5 members in the family and typically have teenagers.

## Campaign Insights
### Deals
- **Cluster 0** and **Cluster 3** responded well to the deals offered.
- However, our **star customers** in **Cluster 1** were not as engaged with the deals.
- **Cluster 2** did not show significant interest in the deals.

### Campaign Participation
- Campaign participation was low across all clusters, with no customers partaking in all campaigns. More targeted and planned campaigns could be beneficial in improving engagement.

## Income vs Spending Patterns
The **Income vs Spending** analysis revealed that:
- **Cluster 0**: High spending with average income.
- **Cluster 1**: High spending with high income.
- **Cluster 2**: Low spending with low income.
- **Cluster 3**: High spending with low income.

Next, the spending patterns were examined across product categories, such as wines, fruits, meat, fish, sweets, and gold, to identify opportunities for targeted marketing strategies.

## Tools & Libraries
This project was built using the following tools and libraries:
- **Python**: The core programming language used.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computing.
- **Scikit-learn**: For performing PCA, scaling, and clustering.
- **Matplotlib & Seaborn**: For visualizations.
- **Sweetviz**: For creating exploratory data analysis (EDA) reports.

## Conclusion
This project provided valuable insights into customer segmentation, helping businesses tailor their marketing efforts. By identifying the distinct characteristics of each customer segment, businesses can develop targeted campaigns, optimize resource allocation, and improve overall customer satisfaction.

This segmentation model can be a powerful tool for marketers looking to boost customer engagement, retention, and sales. The use of unsupervised clustering methods like **Agglomerative Clustering** combined with **dimensionality reduction** via **PCA** ensured that the segments were interpretable and actionable.

The profiling of clusters and the resulting insights allow businesses to focus on the most relevant aspects of their customer base, leading to more personalized and effective marketing strategies.
