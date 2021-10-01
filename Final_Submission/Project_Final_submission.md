# MVP - Movie Revenue prediction using Linear Regression

## Linear Regression and Web Scraping


### Purpose:

We will always have super high budget movies that are box office bombs!

Low Budget Films that became Blockbuster hits!

Build linear regression model to predict the movie revenue using the [boxofficemojo movie dataset](https://www.boxofficemojo.com/) and help the Movie Producers to understand the target movies to invest in.

### Target Clients:
Movie producers, directors, investors would be heavily benefitted by this revenue prediction model


### Data Description:
Using web scraping to get the movie dataset from public websites:

•	[boxofficemojo dataset](https://www.boxofficemojo.com/)

Picked (domestic) movies by MPAA Ratings - G, G/PG, PG, PG-13, R

Target (Y): Domestic_total_revenue

Features (X):
1. Budget
2. Release Year
3. Rank_overall
4. Rank_by_mpaa_rating
5. Runtime
6. Rating

I have done the initial data cleaning and exploratory analysis on this movie dataset

### Modelling:

I. Plotted a pairplot to understand the relationship of the target (Y) with different features (X), and also relationship amongst the features themselves.


## Data Analysis

II. Analysis of features

1. Budget of the movie is almost linearly related to the movie revenue
2. Month of movie release to consider the seasonality changes
3. Movie Genres - Comedy, Action, Adventure, Horror, etc

Original data: 6360 data points + 11 features 

After initial explorations and feature analysis- Final data: 2199 data points + 46 features 

## Algorithms

III. Divide the entire movie dataset into:
    1. Training set (80%)
    2. Holdout set i.e. Test dataset (20%)

IV. Performed Linear Regression
TRAIN R^2 SCORE: 0.331
TEST R^2 SCORE: 0.337


## Improving the Model

### Standardizing the inputs

V. LASSO Regularization

Optimal alpha is: 0.00066
RMSE ERROR IS: 65106880.94
R^2 WITH LASSO IS: 0.4145
RMSE ERROR ON TEST DATA IS: 65725821.63
R^2 WITH LASSO ON TEST DATA IS: 0.4045


### Recommendations:

1. High Budget Movie $$$

2. Summer or Holiday
(Thanksgiving / Christmas)
Blockbuster release

3. Genres
(Animation, Comedy, Action)

4. MPAA Rating PG-13

## Future Work

1. Incorporating more features to train the model better: Enitre Movie Cast - Actors, Producers, Directors; Storyline; Marketing Budget; movie remake, etc.
2. Understanding seasonality changes, new trends due to COVID-19 pandemic.
3. Exploring the movie performances worldwide

Here are some of the helpful plots

## Feature_vs_Target_pairPlot
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/PairPlot_Target_vs_Feature.png)

## Coefficients of Features
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/chart.png)

### Diagnostic Plots

## Plot_predicted_revenue_vs_actual_revenue for Train Set
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/Plot-Fitted_vs_Actual_movie_revenue_TrainSet.png)

## Plot_predicted_revenue_vs_actual_revenue for Test Set
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/Plot-Fitted_vs_Actual_TestSet.png)

## Understanding of the Residuals
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/residuals.PNG)
