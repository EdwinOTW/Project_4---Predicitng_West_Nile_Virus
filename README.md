# Project_4-Predicitng_West_Nile_Virus

This is my first week of work at the Disease And Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE). 

# Problem Statement

Due to the recent epidemic of West Nile Virus in the Windy City,the Disease And Treatment Agency would like to use existing data to build a model and make predictions that the city of Chicago can use when it decides where to spray pesticides.

# Summary of Process

Due to the recent epidemic of West Nile Virus in the Windy City, the agency had the Department of Public Health set up a surveillance and control system. We're hoping it will let us learn something from the mosquito population as we collect data over time. 

In this project, we received 3 DataSets from the data collected by the Department of Public Health surveillance and control systems, built 8 classification models and evaluate the top model which best answer our business needs, to identify whether a location at a certain point in time has the West Nile Virus.

# Process

We were provided with 3 datasets, Weather, Train, Spray Data and 1 dataset for testing our model to see it's predicting capabilities. The Weather DataSet has 2944 Observations and 22 Features, Train DataSet has 10506 Observations and 12 Features, Spray DataSet has 14835 Observations and 4 Features.

We cleaned the data for Weather by filling Null Values with either data collected from the other station or using mean/median of the entire dataset, Train dataset was clean by dropping repeated columns such as Address/Street/Block, Spray was cleaned by filling Null values with the respective time. After cleaning the data, we are have about 94.76%(0) and 5.24%(1) for West Nile Virus. We have a heavily unbalanced dataset which is not an ideal dataset to have for classification problems. From this we are also able to determine that our baseline accuracy is 94.76%.

To explore the data, We plotted time series lineplot to look at time trend regarding the weather and how it affects the observations of West Nile Virus. Then we plotted countplot to look at the relationship between each of the features with respect to the West Nile Virus.
After that we plot a heatmap to determine which are the hotspots where mosquitoes are mostly found and where West Nile Virus is found as well.

We then did some Feature Engineering and built 8 models:
Decision Tree with/without balancing the dataset
Random Forest with/without balancing the dataset
Ada Boost with/without balancing the dataset
Logistic Regression with/without balancing the dataset 
and found out AdaBoost model which has a score of 72.24% in our test data answers our business problem the best.

For the next iteration to improve this model, we can look at running the model again after futher feature engineering and maybe dropping a couple of features that may not have as much significance. Or we can collect larger and more balanced dataset then tune our model again to improve its classification accuracy. 

When the model is accurate enough, we can expand the usage to other States and consider having subreddit auto-warning system. This would warn us of possible West Nile Viruses happening and we would be able to tackle the problem before it surfaces. Prevention is better and more effective than Cure.
