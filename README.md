This assignment analyzes 2016 San Francisco public employee compensation data using k-means and hierarchical clustering. The dataset (Employee_Compensation_SF.csv) includes salary, benefits, and total compensation variables. The analysis focuses primarily on Total Salary and Total Benefits to identify natural groupings among employees.

The workflow begins by importing the data, removing rows with missing values, and excluding non-numeric or categorical variables that are inappropriate for k-means clustering. The remaining numeric variables are standardized using centering and scaling to ensure equal contribution to distance calculations.

Exploratory analysis includes a scatter plot of Total Salary versus Total Benefits using ggplot2, which shows a clear positive relationship between the two variables. An elbow chart is then generated (using BabsonAnalytics.R) to help determine an appropriate number of clusters, suggesting an optimal value of approximately three.

K-means clustering is performed using four clusters with multiple random starts to improve stability. Cluster sizes and centers are examined, and clusters are bound back to the dataset for visualization. A colored scatter plot illustrates how employees are segmented based on compensation patterns.

Hierarchical clustering is also explored. When attempting to compute a distance matrix on the full dataset, R exceeds memory limits due to the large number of observations. To address this, only the first 200 observations are used. Dendrograms are created using average, single, and complete linkage methods; however, the results are not visually informative due to label congestion and the inherent limitations of hierarchical clustering for large datasets.

To run this analysis, ensure that the data file and BabsonAnalytics.R are located in the working directory specified in the setup chunk. Required packages include caret and ggplot2. The final output is rendered as an HTML document.
