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
- Jun is the peak season and October to December are the slack seasons in a year.

2. Where is the best place to rent in Seattle
- Fairmount Park is the highest and Roxhill is the cheapest place to rent in Seattle.

3. What factors correlated with the price
- accommodates,bedrooms,beds,square_feet,bathrooms have strong relationships with price.

4. How can I predict price by variables and the evaluation of the data model.
- I use the variables whose correlation coefficient >0.3 and have low missing values percentage as the independent variables to predict price. 
- Here is the evaluation of the model:Mean squared error is 4200 and R2=0.48.


## Analysis Detail
question 1. When is the peak season for travelling to Seattle
- Jun is the peak season in Seattle: I can see the occupation rate is the lowest and price is the highest in Jun among the year.
- October to December is the slack season in Seattle: The occupation rate is high and price is low.

![image](https://user-images.githubusercontent.com/30916036/129544914-5a0dbdcd-4dd7-4d25-a077-3d3047997d55.png)
![image](https://user-images.githubusercontent.com/30916036/129544958-caced60d-7631-4cb8-b2aa-077bbd63de95.png)


question 2. Where is the best place to live in Seattle
- I can see the big difference between neighbourhood.Fairmount Park is the highest and Roxhill is the cheapest place to rent in Seattle.
![image](https://user-images.githubusercontent.com/30916036/129546727-215b1f65-d48a-4604-a552-79ca79524111.png)


question 3. What impact on price
- From corr analysis,I found accommodates,bedrooms,beds,square_feet,bathrooms,guests_included,reviews_per_month have strong or middle relationship with price.
![image](https://user-images.githubusercontent.com/30916036/129547495-c5f9103b-c4aa-4adb-a9b1-47b92c31ac23.png)

question 4. What is the final data model to predict price
From above corr analysis with price,I choose the variables whose absolute correlation coefficient >0.2 as the independent variables to predict price.However the missing value percentage of square_feet is over 50%,I decide to abondon this variable althougn it have high relationship with price.Here is the final model and evalation of the model.

![image](https://user-images.githubusercontent.com/30916036/129565294-62869f8a-9235-4d93-8380-c7f355e8d97d.png)
