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
1.1 I can see that data period is from 2016-01-04 to 2017-01-02
1.2 We can see only four fields in this table.
1.3 For date field: it’s not date type.We need transfer them to date type if we need calculate
1.4 For price field:it’s not int/float type.We need to transfer them if we need to calculate.There are some missing values in this field.


2. Listing
2.1 There are 91 fields in this table
2.2 Below is the null values percentage for each field in this table.

3. Review
3.1 I can see only  6 fields in this data.There are some missing values in comments.Date is object type,we need transfer them to date type if we need to calculate.

## Data preparation
1. When is the best month for travelling to Seattle
2. Where is the best place to live in Seattle


## Modeling
## Evaluation
