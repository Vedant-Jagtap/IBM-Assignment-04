# IBM-Assignment-04
# Employee Workforce Segmentation

## Project Overview

Employee Workforce Segmentation is a data science project that applies unsupervised machine learning techniques to group employees based on their characteristics, job-related information, satisfaction, compensation, and work experience.

The project uses **K-Means clustering, Hierarchical Clustering, and Principal Component Analysis (PCA)** to identify workforce segments, visualize employee groups, and explore patterns related to employee attrition, department distribution, performance, and retention.

## Project Objectives

- Segment employees into meaningful groups using clustering algorithms.
- Implement K-Means and Hierarchical Clustering.
- Apply PCA to reduce feature dimensions and visualize employee segments.
- Identify clusters with higher historical employee attrition rates.
- Analyze workforce segments across departments and performance ratings.
- Create a workforce analytics dashboard to support HR decision-making.

## Dataset

The project uses the IBM HR Employee Attrition dataset.

- **Number of employee records:** 1,470
- **Original columns:** 35
- **Target analysis:** Workforce segmentation and historical attrition patterns

The dataset contains employee information such as age, department, job role, monthly income, job satisfaction, performance rating, and years at the company.

The `Attrition` column is excluded from the clustering inputs and used afterward to compare historical attrition rates across the resulting clusters.

## Methodology

### 1. Data Preprocessing
- Load and inspect the employee dataset.
- Remove employee identifiers and constant columns from clustering features.
- Handle missing values.
- Encode categorical variables.
- Standardize numerical features.

### 2. K-Means Clustering
- Evaluate different cluster counts using the elbow method and silhouette score.
- Group employees based on similarities in their processed features.
- Compare the characteristics of the resulting clusters.

### 3. Hierarchical Clustering
- Apply agglomerative hierarchical clustering.
- Compare employee groupings and cluster separation.
- Visualize the resulting segments.

### 4. Principal Component Analysis (PCA)
- Reduce the dimensionality of the processed employee data.
- Examine explained variance and the number of components needed to retain 95% of the variance.
- Visualize employee segments using the first two principal components.

### 5. Workforce Analysis
- Compare employee counts across clusters.
- Analyze historical attrition rates by cluster.
- Examine department-level workforce distribution.
- Compare performance-rating distributions.
- Explore employee age, income, satisfaction, and tenure across segments.

### 6. Workforce Analytics Dashboard
Create visualizations showing:
- Employee count by cluster.
- Historical attrition rate by cluster.
- Department distribution by cluster.
- Performance-rating distribution by cluster.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub

## Expected Deliverables

1. **Employee Segmentation Report** — summary of the identified clusters and their workforce characteristics.
2. **PCA Summary** — dimensionality reduction results, explained variance, and cluster visualization.
3. **Workforce Analytics Dashboard** — charts for cluster sizes, department distribution, performance groups, and historical attrition patterns.
4. **Jupyter Notebook** — implementation of preprocessing, clustering, PCA, analysis, and visualizations.

## Business Value

Employee segmentation can help HR teams understand workforce patterns, compare employee groups, and identify segments that may need further investigation or retention support.

Clusters with higher historical attrition rates can be examined alongside department, satisfaction, tenure, and compensation patterns. These findings are exploratory and do not establish the causes of employee attrition.

## Limitations

- Clustering results depend on feature selection, preprocessing, and the chosen number of clusters.
- PCA visualizations may not capture every difference present in the original feature space.
- Historical attrition patterns do not guarantee future employee behavior.
- Cluster membership should not be treated as a definitive measure of an individual employee's risk or performance.

## Conclusion

This project demonstrates how unsupervised machine learning and dimensionality reduction can be applied to HR analytics. K-Means and Hierarchical Clustering are used to explore employee segments, while PCA helps visualize workforce patterns. The resulting analysis supports data-informed workforce exploration and retention discussions.

## Author

Data Science Assignment — Employee Workforce Segmentation
