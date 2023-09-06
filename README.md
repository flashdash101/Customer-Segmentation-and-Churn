# Project README

## Background
This README provides an overview of a customer segmentation analysis project. The analysis aims to uncover valuable insights from two distinct datasets: one focusing on Mall Customer Segmentation and the other on Customer Churn Rate prediction. The project employs data preprocessing, feature selection, K-Means clustering, visualization, and interpretation to derive actionable business insights.

## Customer Segmentation Analysis
### Rationale
The project seeks to identify distinct customer segments based on relevant features, providing a foundation for targeted marketing and product development strategies.

### Features and Preprocessing
For the Mall Customer Segmentation dataset, the selected features include CustomerID, Gender, Age, Annual Income (k$), and Spending Score (1-100). Data preprocessing involves dropping irrelevant columns and retaining the 'Gender' feature as is, rather than one-hot encoding.

### Optimal Number of Clusters
The Elbow Method was employed to determine the optimal number of clusters. It suggests the use of three clusters for meaningful segmentation.

### Cluster Profiles
Clusters were visualized using scatterplots and 3D scatterplots. Two clusters of particular interest were Cluster 1 (high annual income and spending score) and Cluster 3 (low annual income but high spending score).

### Insights
- Females tend to have higher median spending scores than males.
- Age has a relatively weak correlation with spending score.
- Clusters 1 and 3 present opportunities for tailored marketing strategies and product offerings.

## Customer Churn Rate Analysis
### Rationale
This analysis aims to predict customer churn rates based on various customer features and identify factors influencing churn.

### Features
The Churn Rate dataset includes features such as Gender, Senior Citizen, Partner, Dependents, tenure, and more.

### Machine Learning Algorithms
The project employs K-Means Clustering to identify customer segments with different churn behaviors. The optimal number of clusters is determined using the Elbow Method.

### Limitations
- Clustering assumptions may not always align with business realities.
- The choice of the "elbow" point in the Elbow Method can be subjective.
- Only four features were considered; additional features like visit frequency could enhance the analysis.

### Insights
- Different clusters exhibit varying mean values for age, annual income, and spending score.
- Tailored marketing strategies can target specific customer segments based on age, income, and spending score.

## Conclusions
- Gender plays a role in spending patterns, with females spending more than males.
- Younger customers tend to spend more and have higher spending scores.
- Marketing campaigns should consider gender and age demographics.
- Annual income has a weaker correlation with spending score than expected.

The project provides valuable insights for decision-making, product development, and revenue enhancement.

## Future Work
1. Incorporate Timeline Data: Include datasets with timeline information for dynamic churn analysis.
2. Explore Advanced Models: Experiment with various machine learning models beyond K-Means clustering.
3. Integrate External Data: Incorporate economic indicators and social trends for deeper analysis.
4. Refine Segmentation: Improve customer segmentation by incorporating more features and advanced techniques.

## References
- [Elbow method (clustering) Wikipedia](https://en.wikipedia.org/wiki/Elbow_method_(clustering)#:~:text=In%20cluster%20analysis%2C%20the%20elbow,number%20of%20clusters%20to%20use)
- [K-means clustering Wikipedia](https://en.wikipedia.org/wiki/K-means_clustering)

This README provides a concise overview of the project, its methodologies, insights, and future directions. For detailed information and code, please refer to the full project documentation.
