![image](https://user-images.githubusercontent.com/30916036/129551845-5bdab939-e32e-4940-9bd2-613bae7bbbf4.png)

# Introduction
Seattle is a famous place for travelling.I want to have some findings from airbnb seattle data so that I can make good choices to travel there.

# Datasource Overview
My datasource comes from https://www.kaggle.com/airbnb/seattle/data .it include below three datasets:
1. Listings, including full descriptions and average review score
2. Reviews, including unique id for each reviewer and detailed comments
3. Calendar, including listing id and the price and availability for that day

# Results
From data analysis,I have below questions and answers
1. When is the best month for travelling to Seattle
- Jul is the peak season and October to December are the slack seasons in a year.

2. Where is the best place to rent in Seattle
- Fairmount Park is the highest and Roxhill is the cheapest place to rent in Seattle.

3. What factors correlated with the price
- accommodates,bedrooms,beds,square_feet,bathrooms have strong relationships with price.

4. How can I predict price by variables and the evaluation of the data model.
- I use the variables whose correlation coefficient >0.2 and have low missing values percentage as the independent variables to predict price. 
- Here is the evaluation of the model:Mean squared error is 4200 and R2=0.48.
![image](https://user-images.githubusercontent.com/30916036/129658252-a76e13f1-0625-4ea9-83e0-8664ca77dab6.png)



# Data analysis process
## Business Understanding.
From the data analysis I want to get to know below questions
1. When is the best month for travelling to Seattle
2. Where is the best place to rent in Seattle
3. What factors impact the price
4. I want to set model to predict price

## Data Understanding
### Calendar
1. I can see only six fields in this table.For date column: it’s not date type.For price column:it’s not int/float type and it have many missing values.

![image](https://user-images.githubusercontent.com/30916036/129543154-952ace67-4034-4c61-b4c7-20b00f340db7.png)


2. I can see that data period is from 2016-01-04 to 2017-01-02

![image](https://user-images.githubusercontent.com/30916036/129543216-0ab6b2ef-ecf5-41bd-8934-3d5a1666eb44.png)

### Listing
1. There are 92 fields in this table.

![image](https://user-images.githubusercontent.com/30916036/129543469-cb139987-c832-486c-a32e-f494141bfa65.png)

2. Below is the column list whose null values percentage over 20%.I can see some columns like licence ect have high percentage of null values.

![image](https://user-images.githubusercontent.com/30916036/129653862-85f70fc6-d48a-482f-9764-d0f9318f0612.png)


### Review
1. I can see only  6 fields in this data.There are some missing values in comments column.

![image](https://user-images.githubusercontent.com/30916036/129543654-33c1815e-838e-4f17-9199-e0b2192ea9dc.png)

## Data preparation
1. When is the peak season for travelling to Seattle

Note:As data period is from 2016-01-04 to 2017-01-02 in calendar table,there's no meaning to use 2017 data in this table.I only choose data year=2016 as my analysis data.
- Jul is the peak season in Seattle: I can see the occupation rate is the lowest and price is the highest in Jun among the year.
- October to December is the slack season in Seattle: The occupation rate is high and price is low.

![image](https://user-images.githubusercontent.com/30916036/129544914-5a0dbdcd-4dd7-4d25-a077-3d3047997d55.png)
![image](https://user-images.githubusercontent.com/30916036/129544958-caced60d-7631-4cb8-b2aa-077bbd63de95.png)


2. Where is the best place to live in Seattle

- I can see the big difference between neighbourhood.Fairmount Park is the highest and Roxhill is the cheapest place to rent in Seattle.
![image](https://user-images.githubusercontent.com/30916036/129546727-215b1f65-d48a-4604-a552-79ca79524111.png)


3. What impact on price
- From corr analysis,I found accommodates,bedrooms,beds,square_feet,bathrooms,guests_included,reviews_per_month have strong or middle relationship with price.
Below is the column list whose correlation coefficient over 0.2.

![image](https://user-images.githubusercontent.com/30916036/129654853-de8fb647-b957-4e87-abac-b5b0bb8db365.png)


## Modeling and Evaluation
From above corr analysis with price,I choose the variables whose absolute correlation coefficient >0.2 as the independent variables to predict price.However the missing value percentage of square_feet is over 50%,I decide to abondon this variable althougn it have high relationship with price.Here is the evalation of the model.

![image](https://user-images.githubusercontent.com/30916036/129565294-62869f8a-9235-4d93-8380-c7f355e8d97d.png)
