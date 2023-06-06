# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The project's aim was to access data using APIs (in this case, Citybik, Yelp and Foursquare), clean and transform data using Python, and load data into a database. Then, perform EDA, using both statistics and visualizations, identify trends and patterns in data using statistical models and interpret those results.

The goal was to predict AVAILABLE BIKES in bike stops in Montreal using Station Numbers, Latitude and Longitude, Average rating of parks, Total rating count and Number of parks that are 1,000m around the bike station. 

## Process
### 1. Explored the structure of the APIs and choose Montréal as the city
### 2. Gathered data from CityBik, Foursquare and Yelp
### 3. Joined and cleaned gathered data
### 4. Exploratory Data Analysis
### 5. Regression Model Development
### 6. Model Evaluation and Interpretation

## Results
While accessing data through the Citybik API was straightforward, working with the Foursquare and Yelp APIs presented some challenges. Unpacking the nested dictionaries and transforming the data into a dataframe required a significant amount of time and effort. However, the Foursquare API proved advantageous with its larger number of total ratings, providing increased validity to the ratings. Moreover, the inclusion of category IDs in the Foursquare API simplified the filtering process, making it more efficient and user-friendly. On average, Foursquare had 107 reviews, surpassing Yelp's average of 61 reviews.

The project utilized Ordinary Least Squares (OLS) regression models to predict the number of available bikes in bike stations. However, the results from all three models indicated that none of the variables were successful in accurately predicting the availability of bikes in specific bike stations. Interestingly, among the three models, the one incorporating data solely from Yelp yielded the best performance.

## Challenges 
### 1. Limited Data Availability
Obtaining comprehensive and reliable data on Montreal parks, including customer reviews, posed a challenge due to data availability constraints.

### 2. Different defitinions of locations
Both Yelp and Foursquare were used to gather data for parks in Montreal. However, these platforms have varying definitions of what constitutes a park. Some locations identified as parks in Yelp may not be recognized as parks in Foursquare and vice versa, leading to potential discrepancies in the data.

### 3. Data for bike stations was collected only in one instance
Data for bike stations was collected only once, specifically on a Friday around 4 pm. Considering that this time corresponds to typical working hours when fewer people may be utilizing bikes, the availability of bikes around parks during this specific instance might be lower than at other times.

## Future Goals
### - Conduct Deeper Analysis: 
Explore additional variables and gathering more comprehensive data for bike stations. This includes extending the data collection period to cover longer durations, capturing different times of the day to account for variations in bike usage patterns.
### - Perform External Validation: 
Validate the regression model's findings by comparing them with external data sources.
### - Fine-tune the Model: 
Refine the regression model by incorporating additional variables or considering different modeling techniques to improve its predictive power and accuracy.