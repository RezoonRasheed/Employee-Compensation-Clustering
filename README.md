# Employee Compensation Clustering Analysis

## Project Overview
This assignment analyzes 2016 San Francisco public employee compensation data using k-means and hierarchical clustering techniques. The goal is to identify natural groupings among employees based on compensation patterns, with a primary focus on Total Salary and Total Benefits.

## Dataset
- **File:** Employee_Compensation_SF.csv  
- **Scope:** Public employees in San Francisco (2016)  

**Key Variables**
- Total Salary  
- Total Benefits  

The dataset includes salary, benefits, and total compensation variables. Non-numeric and categorical variables are excluded for clustering suitability.

## Objectives
- Identify natural employee segments based on compensation  
- Apply and compare k-means and hierarchical clustering methods  
- Determine an appropriate number of clusters using the elbow method  
- Visualize compensation-based groupings for interpretation  

## Methodology
- Data imported and cleaned by removing missing values  
- Numeric variables standardized using centering and scaling  
- Exploratory analysis conducted using scatter plots of Total Salary vs. Total Benefits  
- Elbow chart used to identify an optimal number of clusters  
- K-means clustering performed with multiple random starts  
- Cluster assignments visualized through colored scatter plots  
- Hierarchical clustering explored on a reduced sample due to memory constraints  

## Tools & Technologies
- R / Quarto (.qmd)  
- ggplot2  
- caret  
- BabsonAnalytics.R  

## Repository Structure
- Assignment_Clustering.qmd # Main analysis file
-  Employee_Compensation_SF.csv # Dataset
-  BabsonAnalytics.R # Supporting functions
-  README.md # Project documentation

## How to Run
1. Place the dataset and `BabsonAnalytics.R` in the working directory  
2. Open the `.qmd` file in RStudio  
3. Install required packages (`caret`, `ggplot2`)  
4. Knit the file to HTML to view results  

## Key Outcomes
- Clear segmentation of employees based on compensation levels  
- Evidence of a strong relationship between salary and benefits  
- Practical comparison of clustering techniques and their limitations  

## Author
Rezoon Rasheed  
MS in Business Analytics
