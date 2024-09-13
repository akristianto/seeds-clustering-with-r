# K-Means Clustering on Seeds Dataset

## Project Overview

This project uses the **Seeds Dataset** from the UCI Machine Learning Repository, available [here](https://archive.ics.uci.edu/dataset/236/seeds). The dataset contains measurements of geometrical properties of kernels belonging to three different varieties of wheat. The goal of this project is to perform a brief **Exploratory Data Analysis (EDA)** followed by the application of **K-Means Clustering** to group the seeds into distinct clusters based on their features.

## Objectives
- Conduct a short **Exploratory Data Analysis (EDA)** to understand the dataset's structure, distribution, and relationships between the variables.
- Apply the **K-Means Clustering** algorithm to partition the data into clusters.

## Dataset Description

The **Seeds** dataset consists of seven numerical attributes derived from geometrical properties of kernels:
1. Area of the kernel.
2. Perimeter of the kernel.
3. Compactness of the kernel.
4. Length of the kernel.
5. Width of the kernel.
6. Asymmetry coefficient of the kernel.
7. Length of the kernel groove.

The dataset contains measurements for three wheat varieties. However, this information will not be used during clustering, as K-Means is an unsupervised learning algorithm.

## Project Structure

The notebook is organized into the following sections:

1. **Introduction**: A brief overview of the dataset and project objectives.
   
2. **Data Loading**: Importing and inspecting the dataset (checking its dimensions, summary statistics, and identifying missing values).

3. **Exploratory Data Analysis (EDA)**:
   - Summary statistics such as mean, median, and standard deviation for each variable.
   - Visualizations including histograms and pairwise scatterplots to explore distributions and relationships.
   - Correlation matrix to analyze linear relationships between variables.

4. **Data Preprocessing**:
   - Standardization of features using `scale()` to normalize the data and prepare it for K-Means clustering.

5. **K-Means Clustering**:
   - Application of the **K-Means** algorithm to the dataset using `kmeans()` in R.
   - **Elbow Method** to determine the optimal number of clusters.
   - Visualization of the clustering results using 2D scatter plots (using PCA for dimensionality reduction if needed).

6. **Conclusion**: Summary of clustering results and insights gained from the analysis.

## Requirements

To run the analysis, you'll need the following R packages:

- `ggplot2`
- `dplyr`
- `cluster`
- `factoextra`

You can install the required packages by running the following in your R environment:

```r
install.packages(c("ggplot2", "dplyr", "cluster", "factoextra"))
```
