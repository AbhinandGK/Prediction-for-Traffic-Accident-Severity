# Prediction for Traffic Accident Severity

## Introduction 

### Background
Traffic accidents are a significant source of deaths, injuries, property damage, and a major concern for public health and traffic safety. Accidents are also a major cause of traffic congestion and delay. Effective management of accident is crucial to mitigating accident impacts and improving traffic safety and transportation system efficiency. The effective treatment of road accidents and thus the enhancement of road safety is a major concern to societies due to the losses in human lives and the economic and social costs. Tremendous efforts have been dedicated by transportation researchers and practitioners to improve road safety.

### Problem
The world as a whole suffer due to car accidents. Accurate predictions of severity can provide crucial information for emergency responders to evaluate the severity level of accidents, estimate the potential impacts, and implement efficient accident management procedures. Previous years countrywide car accident dataset can be used to determining severity prediction.

## Data acquisition and cleaning

### Data sources
U.S countrywide [car accident dataset data](https://www.kaggle.com/sobhanmoosavi/us-accidents) can be found in Kaggle datasets. Here countrywide car accident dataset, which covers 49 states of the USA is used for the analysis. The accident data are collected from February 2016 to June 2020, using two APIs that provide streaming traffic incident (or event) data. These APIs broadcast traffic data captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, there are about 3.5 million accident records in this dataset. Here I used the first 5 lakh rows for this Analysis. 

## Feature Selection
After data Cleaning there were 3414252 samples and 38 features in the data. Upon examining the meaning of each feature, it was clear that there was some redundancy in the features. From these highly correlated features, only one was kept, others were dropped from the dataset. After all, 23 features were selected.


