# Introduction
Seattle is a famous place for travelling.I want to have some findings from airbnb seattle data so that I have make good choice to travel there.

# Datasource Overview
I use following datasets comes from https://www.kaggle.com/airbnb/seattle/data .it include below three datasets:
1. Listings, including full descriptions and average review score
2. Reviews, including unique id for each reviewer and detailed comments
3. Calendar, including listing id and the price and availability for that day

# Results
From data analysis,I have below questions and answers
1. When is the best month for travelling to Seattle
2. Where is the best place to live in Seattle
3. What factors impact the price


# Data analysis process
## Business Understanding.
From the data analysis I want to get to know below questions
1. When is the best month for travelling to Seattle
2. Where is the best place to live in Seattle
3. What factors impact the price

## Data Understanding
1. Calendar
1.1.   We can see only six fields in this table.For date field: it’s not date type.For price field:it’s not int/float type.We need to transfer them if we need to calculate.There are some missing values in this field.

![image](https://user-images.githubusercontent.com/30916036/129543154-952ace67-4034-4c61-b4c7-20b00f340db7.png)

1.2.   I can see that data period is from 2016-01-04 to 2017-01-02

![image](https://user-images.githubusercontent.com/30916036/129543216-0ab6b2ef-ecf5-41bd-8934-3d5a1666eb44.png)

2. Listing
2.1.   There are 92 fields in this table.

![image](https://user-images.githubusercontent.com/30916036/129543469-cb139987-c832-486c-a32e-f494141bfa65.png)

2.2.   Below is the null values percentage for each field in this table.

![image](https://user-images.githubusercontent.com/30916036/129543549-bb6ac72f-0739-456b-a72e-3e6417d5f544.png)

3. Review
3.1.   I can see only  6 fields in this data.There are some missing values in comments.

![image](https://user-images.githubusercontent.com/30916036/129543654-33c1815e-838e-4f17-9199-e0b2192ea9dc.png)

## Data preparation
1. When is the best month for travelling to Seattle
2. Where is the best place to live in Seattle


## Modeling
## Evaluation
