# Seattle Airbnb Data Analysis Introduction
# Project Overview
Seattle is a famous place for travelling.I want to have some findings from airbnb seattle data so that I have make good choices to travel there. 


# Datasource Overview
I use following datasets comes from https://www.kaggle.com/airbnb/seattle/data .it include below three datasets:
1. Listings, including full descriptions and average review score
2. Reviews, including unique id for each reviewer and detailed comments
3. Calendar, including listing id and the price and availability for that day


# Analysis tool
The project use Python3 and below package installed to do the analysis.
1. Numpy
2. Pandas
3. Matplotlib
4. sklearn

# Code
pls check Seattle Airbnb data analysis.ipynb in this repository.


# Results
From data analysis,I have below questions and answers
1. When is the best month for travelling to Seattle
- Jun is the peak season and October to December are the slack seasons in a year.

2. Where is the best place to rent in Seattle
- Fairmount Park is the highest and Roxhill is the cheapest place to rent in Seattle.

3. What factors correlated with the price
- accommodates,bedrooms,beds,square_feet,bathrooms have strong relationships with price.

4. How can I predict price by variables and the evaluation of the data model.
- I use the variables whose correlation coefficient >0.2 and have low missing values percentage as the independent variables to predict price. 
- Here is the evaluation of the model:Mean squared error is 4200 and R2=0.48.


Pls get to know the full analysis from my post:https://github.com/luobohaohao/data-2/blob/gh-pages/Final%20Post.md
