
# Project: House Sales Analysis in King County, USA

This project aims to analyze house sales data for King County, which includes Seattle. The dataset contains information about houses sold between May 2014 and May 2015. The goal is to explore various features of the dataset and build predictive models to understand the factors influencing house prices.


## Data Description

The dataset consists of 21,613 rows and 21 columns containing various features related to the houses. Here's a description of each column:

id: A unique identifier for each house.

date: The date the house was sold.

price: The price of the house. This is the target variable we aim to predict.

bedrooms: The number of bedrooms in the house.

bathrooms: The number of bathrooms in the house.

sqft_living: The square footage of the living space in the house.

sqft_lot: The square footage of the lot the house sits on.

floors: The total number of floors in the house.

waterfront: Whether the house has a view of the waterfront (0: No, 1: Yes).

view: Whether the house has a good view (0: No, 1: Yes).

condition: The general condition of the house (overall rating).

grade: The overall grade given to the house based on King County grading systems.

sqft_above: The square footage of the house above the basement.

sqft_basement: The square footage of the basement in the house.

yr_built: The year the house was built.

yr_renovated: The year the house was last renovated (if applicable).

zipcode: The zip code of the location.

lat: The latitude coordinate of the house.

long: The longitude coordinate of the house.

sqft_living15: The square footage of the living space in 2015 (might be affected by renovations).

sqft_lot15: The square footage of the lot in 2015 (might be affected by renovations).
## Data Cleaning

1- The Unnamed: 0 column was dropped as it's not relevant to the analysis.

2- Missing values in the bedrooms and bathrooms columns were imputed using the mean values since they are numerical features.
## Exploratory Data Analysis (EDA)

We performed various tasks to understand the data and identify trends:

1- We checked for missing values in each column.

2- We calculated descriptive statistics to summarize the data (mean, median, standard deviation, etc.).

3- We visualized the distribution of features to identify patterns and outliers.

4- We analyzed the correlations between features and the target variable (price) to understand which features might be most influential.
## Modeling

We explored different machine learning models to predict house prices:

1- Linear Regression: We trained a linear regression model using various features to predict the price of a house.

2- Polynomial Regression with Pipeline: We created a pipeline that incorporates feature scaling, polynomial feature creation, and linear regression to improve model performance.
## Evaluation

We evaluated the performance of our models using the following metrics:

1- Mean Squared Error (MSE): Measures the average squared difference between the predicted and actual house prices. Lower MSE indicates better model fit.

2- R-squared: Represents the proportion of variance in the target variable (price) explained by the model. Higher R-squared indicates better model performance.
## Results

The pipeline model using polynomial features achieved a higher R-squared (0.746) and lower MSE compared to the linear regression model (R-squared: 0.658, MSE: 46142241414.675). This suggests that the pipeline model captures more of the variance in house prices and generates predictions closer to the actual values.
## Conclusion

This project analyzed house sale prices in King County, USA, using various data cleaning, exploration, and modeling techniques. We built and evaluated models to predict house prices, achieving an R-squared of 0.746 with a pipeline model that incorporates polynomial features. This project provides a starting point for further exploration and refinement of house price prediction models.