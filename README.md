# Airbnb-Price-Prediction

This project is about price prediction of Airbnb rental. I used NYC's Airbnb dataset for this project from [Kaggle](https://www.kaggle.com/c/lalapaceairbnb/data). This dataset has 30k observations and 103 features. The dataset includes detail of listing such as name, description, location and so on. It also has detail about the listing such as bedrooms, bathrooms, bed type, shared or not and other related information.

Linear Regression and Random Forest Regression were used to predict the price.


### Data Cleaning

Removed some columns which had greater than 30% missing values or didn't have meaningful insight
Set dummie varible for NYC boroughs, room type and property type as they have multiple categories

### Exploratory Data Analysis

I asked a few questions for exploratory analysis which are the following:

What is the price per borough? and I found Manhattan has a maximum price for Airbnb rental and then, Brooklyn, Queens, Staten Island, and the Bronx have rental pricing in decreasing order.

What is the price according to room type (private/home/apt/shared) for all boroughs? I noticed that Manhattan has a maximum price for Entire home/apt and Private room rental whereas Staten Island has a maximum price for Shared room rental. On the contrary, the Bronx has a low rental price for all room types.

What is the price for bed types for all boroughs? From the graph(3rd graph in the notebook), we can see a real bed has a maximum price in all boroughs. However, Manhattan has an equal price for all other bed types (Airbed/fulton/pull-out sofa/couch).

What is the price for accommodates? I noticed Rental price is increasing according to accommodates, and it makes sense because if we stay longer, we have to pay a high price.

### Prediction model

I have implemented two machine learning models, Linear Regression and Random Forest Regression for price prediction. From these models, Random Forest Regression works well with 82% accuracy rate whereas Linear Regression performs very poorly.
