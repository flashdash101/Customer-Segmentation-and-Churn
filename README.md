# Project README

## Background
In this comprehensive report, I delve into my extensive findings, rigorous analysis, and the meticulous methodology employed to construct this report. My analysis hinges on two distinct datasets: one for Customer Segmentation of Mall Customers and another for Customer Churn analysis based on various features.

## Customer Segmentation Analysis
### Rationale
The primary objective of this project is to unearth unique customer segments to drive targeted marketing strategies and inform product development.

### Features
- Mall Segmentation Dataset: CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)
- Churn Rate Dataset: Customer ID, Gender, Senior Citizen, Partner, Dependents, Tenure, Phone Service, Multiple Lines, Internet Service, Online Security, Online Backup, Device Protection, Tech Support, Streaming TV, Streaming Movies, Contract, Paperless Billing, Payment Method, Monthly Charges, Total Charges, Churn

### Methodology
#### Mall Segmentation
- **Data Preprocessing**: CustomerID was dropped, and 'Gender' was retained in its original form.
- **Feature Selection**: Selected Gender, Age, Spending Score, and Annual Income for analysis.

#### Scaling
- Scaling applied for multivariate clustering to ensure no feature dominates others.

#### Machine Learning
- K-Means Clustering used for Mall Segmentation.
- The optimal number of clusters determined using the Elbow Method, resulting in 3 clusters.

![image](https://github.com/flashdash101/Customer-Segmentation-and-Churn/assets/97402685/a8a261f4-0993-45c5-9714-628b0200f319)



#### Visualizations
- A rich array of visualizations including scatterplots, 3D scatterplots, histograms, boxplots, and KDE plots employed.
<img src="https://github.com/flashdash101/Customer-Segmentation-and-Churn/assets/97402685/503d9062-9e0a-42b5-9d1c-9b9b76c210ab" width="250" height="250"> <img src="https://github.com/flashdash101/Customer-Segmentation-and-Churn/assets/97402685/8e4cecce-74c9-4e6d-8b6f-2169c71bd78c" width="250" height="250"><img src="https://github.com/flashdash101/Customer-Segmentation-and-Churn/assets/97402685/e9b7d0ea-6dac-44e6-8b1d-988877878912" width= "250" height = "250">


### Insights
- Median spending score for females is approximately 50, while for males, it's around 75, signifying gender-based spending disparities.
- Age exhibits a relatively weak correlation with spending score (-0.12).
- Cluster 3 predominantly comprises younger customers with lower income but higher spending scores.

### Customer Churn Rate Analysis
#### Methodology
- K-Means Clustering employed.
- Elbow Method indicated 4 or 5 clusters as optimal.

#### Visualizations
- Creation of 3D scatterplots to visualize clusters using age, income, and spending score.
- Mean values analyzed for age, income, and spending score within each cluster.

### Insights
- Cluster 0, characterized by a higher mean age (mean: 60.2), displays negative mean values for annual income (mean: $26.4k) and spending score (mean: 23.7), signifying older customers with lower spending tendencies.
- Cluster 3, despite a younger mean age (mean: 30.9) and lower income, boasts positive mean values for annual income (mean: $76.5k) and spending score (mean: 81.2), indicating younger customers with higher spending scores.

## Conclusions
- Gender exerts a significant influence on spending patterns.
- Age's correlation with spending score is weak, implying the role of other factors.
- Clusters 1 and 3 represent compelling business opportunities for targeted marketing campaigns.

## Further Statistical Insights
### Mall Segmentation
- **Gender and Spending Patterns**: Median spending score for females: 50, males: 75.
- **Age and Spending Behavior**: Age exhibits a weak correlation with spending score (-0.12).
- **Cluster Characteristics**: Cluster 3 comprises younger customers with lower income but higher spending scores.

### Customer Churn Rate Analysis
- **Cluster Analysis**: Cluster 0 consists of older customers with lower income and spending scores, while Cluster 3 comprises younger customers with higher income and spending scores.
- **Gender Composition**: Cluster 3 is predominantly (60%) female, while Cluster 1 is evenly split between genders.

## Business Recommendations
- **Gender-Based Marketing**: Tailor marketing strategies based on gender, acknowledging that females tend to spend more despite slightly lower income.
- **Age-Specific Campaigns**: Design age-specific marketing campaigns to resonate with younger customers who exhibit higher spending scores.
- **Target Clusters**: Focus marketing efforts on Clusters 1 and 3, where opportunities for increased sales revenue are prominent.
  - Cluster 1: Balanced gender distribution, highest income, and spending scores.
  - Cluster 3: Predominantly younger females with strong spending propensity.

## Future Work
1. **Incorporate Timeline Data**: Integrate datasets with timeline information for dynamic churn analysis, tracking trends over time.
2. **Explore Advanced Models**: Experiment with advanced machine learning models beyond K-Means clustering for improved segmentation accuracy.
3. **Integrate External Data**: Include economic indicators and social trends to enhance analysis depth.
4. **Refine Segmentation**: Enhance customer segmentation by incorporating additional features and advanced clustering techniques.
5. **Incorporate Behavior Data**: Consider transactional data, visit frequency, and browsing patterns for a comprehensive understanding of customer behavior.

## Limitations
- Clustering assumptions might not always align with real-world business dynamics.
- The Elbow Method is subjective and not always definitive.
- Limited to 4 features; incorporating additional data could provide deeper insights.
- Sensitivity of K-Means clustering to initial centroids can lead to variable results.
- Interpretability of clusters might be challenging, especially in multivariate analysis.

## References
- [Elbow Method (Clustering) Wikipedia](https://en.wikipedia.org/wiki/Elbow_method_(clustering))
- [K-Means Clustering Wikipedia](https://en.wikipedia.org/wiki/K-means_clustering)
