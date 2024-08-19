# Restaurant Rating Prediction Capstone Project

## Introduction
This project aims to develop a machine learning model to predict the rating of a restaurant based on various variables such as location, price, number of reviews, and more. The ability to predict the success of a restaurant can help determine the best possible locations and factors that contribute to a thriving business in the highly competitive restaurant industry.

## Data Acquisition
The data for this project was obtained using the Yelp API, specifically the business search endpoint. The following variables were selected for each restaurant:
- City
- Price
- Number of Reviews
- Rating
- Latitude
- Longitude

Approximately 500 restaurants were collected from each of the four states: California, Nevada, Utah, and Arizona, resulting in a total of nearly 2,000 places to explore.

## Exploratory Data Analysis
The initial analysis of the data revealed that the distribution of ratings and the correlation between variables were relatively uniform across all four states. However, the correlations between the selected variables did not appear to be strong enough to provide a reliable prediction of restaurant ratings.

## Clustering
Two clustering approaches were employed to visualize the distribution of restaurants:

1. **Statewide Clustering**: The first attempt focused on displaying the distribution of restaurants across the four states.

2. **City-level Clustering**: The second approach narrowed down the analysis to restaurants located within California. This process was repeated for each city, with the resulting clusters primarily represented by the number of reviews. The clusters were color-coded as follows:
   - Red: Low number of reviews
   - Blue: Medium number of reviews
   - Green: High number of reviews

## Predictive Modeling
Two machine learning algorithms were used to predict the rating of each restaurant:

1. **Multiple Linear Regression**: This model was employed to capture the linear relationships between the variables and the restaurant ratings.

2. **Support Vector Machine (SVM)**: SVM was used as an alternative approach to predict the ratings based on the available features.

However, the results of both models indicated that the predictions were not sufficiently accurate, suggesting that the selected variables alone may not be enough to reliably predict restaurant ratings.

## Conclusions and Next Steps
The clustering analysis provided valuable insights into the distribution of restaurants based on price and the number of reviews across different states and cities. However, the predictive models did not perform well in terms of accurately predicting restaurant ratings. This could be attributed to the lack of strong correlations between the selected variables and the limited dataset size.

To improve the predictive performance, the following steps can be considered:
1. Collect a larger dataset with more restaurants and potentially additional relevant variables.
2. Partition the data into more equal-sized subsets to test the variables and their impact on the prediction.
3. Explore and incorporate variables that are more directly related to the problem at hand.

By refining the data collection process, selecting more relevant variables, and expanding the dataset, the predictive model's accuracy can potentially be enhanced, providing more reliable insights into the factors that contribute to a restaurant's success. 