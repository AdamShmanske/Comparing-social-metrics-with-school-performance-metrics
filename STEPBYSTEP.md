# Excel Step-by-Step Description

## General
1. Data from The Opportunity Atlas, Baltimore City Public Schools Open Data, processed data from Professor Shimano
2. Matched SAT scores to tracts using data from Professor Shimano
3. Used tracts from Opportunity Atlas to convert partial tracts from Professor Shimano's data to full tracts
4. Used VLOOKUP function to compile all data from Opportunity Atlas alongside testing data

## Cluster Analysis
1. Copied compiled data into separate tab
2. Found mean and standard deviation for each social metric
3. Used STANDARDIZE function to find z-values
4. Randomly chose three schools for placeholder anchor points, set up table using VLOOKUP function
5. Used SUMXMY2 to find distance of each point from anchor points
6. Found minimum distance to determine which anchor point each school was closest to (using MIN function)
7. Used MATCH function to pair minimum distance to specific anchor point
8. Used VLOOKUP to match anchor point to the name of specific anchor point
9. Used SUM function to find the sum of the minimum distance column
10. Used SOLVER tool to minimize the sum-value, constraints were (<=29, >=0, int)
11. Repeated same steps for partial cluster analysis, but only used percentage non-white and teenage birth rate for social metrics

## Linear Regression
1. Copied compiled data into seperate tab
2. Use Data Analysis linear regression tool with average SAT data and household income to create simple linear regression equation for this 1 variables.
    -Repeat using teen birth rate, incarceration rate, and % nonwhite
3. Select average SAT data and household income and insert scatterplot to graphically represent these 2 values against each other.
4. Using chart design, insert linear trendline, linear equation, R-Squared value, and axis titles on graph.
    -Repeat using teen birth rate, incarceration rate, and % nonwhite
5. Analyze R-Squared and P-value for each simple linear regression to determine if any are statistically significant
6. Use Data Analysis linear regression tool with average SAT data and household income, teen birth rate, incarceration rate, and % nonwhite to create a multiple linear regression analysis for these 4 variables.
7. Analyze R-Squared, P-Value, and Significance F value for multiple linear regression in order to determine the statistical significance of the analysis and each individual variable.
8. Use multiple linear regression coefficients to create a predictive equation that uses an intercept and all 4 variables in order to predict SAT scores.
9. Select observation number and residuals and insert a clustered column graph to graphically display residual values for each observation point.
10. Match true SAT scores (from raw data), predictive SAT scores from residual output, and observations.
11. Insert line chart using true SAT scores, predictive SAT scores, and observations to graphically display predicted vs actual values for each observation. 





