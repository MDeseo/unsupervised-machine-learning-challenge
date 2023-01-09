# Myopia Clusters

In this assignment, unsupervised learning is applied by fitting data to a model and using clustering algorithms to place data into groups. Then, a visualisation was created that showed the findings. 

## Background

A medical research company is interested in finding better ways to predict myopia, or nearsightedness. When training on the whole dataset, the team has tried—and failed—to improve the classification model. However, there might be distinct groups of patients that would be better to analyse separately. So, this assignment explored using unsupervised learning.

## Instructions

This activity is broken down into four parts: 

* Part 1: Prepare the Data

* Part 2: Apply Dimensionality Reduction 

* Part 3: Perform a Cluster Analysis with K-means

* Part 4: Make a Recommendation 

### Part 1: Prepare the Data

1. Read `myopia.csv` into a Pandas DataFrame.

2. Remove the "MYOPIC" column from the dataset.

3. Standardise your dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

### Part 2: Apply Dimensionality Reduction

1. Perform dimensionality reduction with PCA. The desired **explained variance** was determined `PCA(n_components=0.90)` that preserves 90% of the explained variance in dimensionality reduction.

2. Further reduce the dataset dimensions with t-SNE and visually inspect the results by running t-SNE on the principal components, which is the output of the PCA transformation. 

3. Create a scatter plot of the t-SNE output and determine if there are distinct clusters?

### Part 3: Perform a Cluster Analysis with K-means

Create an elbow plot to identify the best number of clusters:

* Use a `for` loop to determine the inertia for each `k` between 1 through 10. 

* If possible, determine where the elbow of the plot is, and at which value of `k` it appears.

### Part 4: Make a Recommendation

Based on your findings, a brief (one or two sentences) recommendation was made. Can the patients be clustered? If so, into how many clusters? 

- - -

## References

Reduced dataset from [Orinda Longitudinal Study of Myopia conducted by the US National Eye Institute](https://clinicaltrials.gov/ct2/show/NCT00000169)

- - -

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.