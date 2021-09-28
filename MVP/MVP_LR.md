# MVP - Movie Revenue prediction using Linear Regression

## Linear Regression and Web Scraping


### Purpose:

Build linear regression model to predict the movie revenue using the [boxofficemojo movie dataset](https://www.boxofficemojo.com/) and understand the driving parameters


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

II. Divided the entire movie dataset into:
    1. Training set (80%)
    2. Holdout set i.e. Test dataset (20%)
    

### Findings:

1. Budget of the movie is almost linearly related to the movie revenue

Here are some of the helpful plots

Feature_vs_Target_pairPlot
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/PairPlot_Target_vs_Feature.png)

Plot_predicted_revenue_vs_actual_revenue
![](https://github.com/chetana-vyas/Linear_Regression/blob/project-proposal/Images/Plot-Fitted_vs_Actual_TestSet.png)

All the following modelling in done on the Training dataset

1. Built a Linear Regression model

The model shows that movie budget is related to the movie box office total domestic revenue.
