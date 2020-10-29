# Excel Step-by-Step Description

## General
1. Data from The Opportunity Atlas, Baltimore City Public Schools Open Data, data from Professor Shimano
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
1. 




