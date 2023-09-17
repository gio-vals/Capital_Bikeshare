# Capital Bikeshare

Capital Bikeshare would like to find out how many bicycles need to be ready at a given time in the Washington, D.C. market.

## Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Statsmodels
- Scipy
- Scikit-learn

## Overview
This project is aimed at analyzing bike-sharing data from Capital Bikeshare to understand patterns and factors affecting bike rentals. Below are the step-by-step tasks performed in this analysis:

1. Importing Libraries: Import necessary libraries for data analysis and visualizations.
2. Data Loading and Inspection: Load the bike-sharing dataset (e.g., dc_bikes.csv) 

3. Data Preprocessing: 
Change the first column to the datetime data type by parsing it using parse_dates=['datetime'].
Extract features like hour, day of the week, month, and year from the datetime column into their own columns for analysis.
4. Exploratory Data Analysis (EDA): Examine whether the bicycle count shows any time-related patterns. Plot small sections of the data over time and explore the 'part+of_day' influence to bike rentals.
5. Error Metrics on a Naive Forecast: Calculate error metrics for a 'naive' forecast, where the count from the previous year is used to predict the next year's count. Evaluate how far off the naive prediction is from the actual counts.
6. Feature Selection and Linear Regression Models: Evaluate which features (temp, atemp, humidity, windspeed) to include in the linear regression model.
Fit various linear regression models with different sets of features and evaluate their R-squared values.
Select the final model with the best R-squared value.
7. Hypothesis Testing (A/B Testing): Perform hypothesis testing to check if there is a significant difference between the 'temp' and 'atemp' columns using t-test statistics.
8. K-Means Clustering (Unsupervised Learning): Create a subset of the dataframe with relevant columns for clustering and standardize the data to account for differences in magnitude. Use the elbow method to determine the optimal number of clusters. Perform K-means clustering with the selected number of clusters.
Visualize the clustering results and compare them with the 'weather' column.

## Getting Started
Follow these steps:

1. Clone the Repository: Clone this GitHub repository to your local machine.

2. Install Dependencies: Ensure you have the required Python libraries installed. You can install them using the following command:
``````
pip install pandas numpy matplotlib seaborn plotly statsmodels scipy scikit-learn
``````
For Jupyter notebooks :
``````
!pip install pandas numpy matplotlib seaborn plotly statsmodels scipy scikit-learn
``````
3. Data File: A .csv file is stored in the /data folder.

4. Run the Code

5. While running the code a new csv files will be created in the data folder.


## Project Output
The project output includes data analysis and visualization in the Jupyter Notebook, insights into bike rental patterns and factors affecting rentals, as well as a Python codebase that can be adapted for similar data analysis projects.