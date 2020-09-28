# Prediction for Traffic Accident Severity

## Introduction 

### Background
Traffic accidents are a significant source of deaths, injuries, property damage, and a major concern for public health and traffic safety. Accidents are also a major cause of traffic congestion and delay. Effective management of accident is crucial to mitigating accident impacts and improving traffic safety and transportation system efficiency. The effective treatment of road accidents and thus the enhancement of road safety is a major concern to societies due to the losses in human lives and the economic and social costs. Tremendous efforts have been dedicated by transportation researchers and practitioners to improve road safety.

### Problem
The world as a whole suffer due to car accidents. Accurate predictions of severity can provide crucial information for emergency responders to evaluate the severity level of accidents, estimate the potential impacts, and implement efficient accident management procedures. Previous years countrywide car accident dataset can be used to determining severity prediction.

## Data acquisition and cleaning

### Data sources
U.S countrywide [car accident dataset data](https://www.kaggle.com/sobhanmoosavi/us-accidents) can be found in Kaggle datasets. Here countrywide car accident dataset, which covers 49 states of the USA is used for the analysis. The accident data are collected from February 2016 to June 2020, using two APIs that provide streaming traffic incident (or event) data. These APIs broadcast traffic data captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, there are about 3.5 million accident records in this dataset. Here I used the first 5 lakh rows for this Analysis. 

### Feature Selection
After data Cleaning there were 3414252 samples and 38 features in the data. Upon examining the meaning of each feature, it was clear that there was some redundancy in the features. From these highly correlated features, only one was kept, others were dropped from the dataset. After all, 23 features were selected.

### Exploratory Data Analysis
Calculation of target variable
The characteristics data set contains information on the time, place, and weather and lighting conditions and type of intersection where it occurred. An initial analysis of the data was performed for the selection of the most relevant features for this problem, reducing the size of the dataset and avoiding redundancy. With this process the number of features was reduced from 38 to 20.

## Predictive Modelling

Different classification algorithms have been tuned and built for the prediction of the level of accident severity. These algorithms provided a supervised learning approach predicting with certain accuracy and f1 score. These two properties have been compared in order to determine the best suited algorithm for his problem. Here preprocessing is done by standard scaler tool from scikitlearn library. After that the sample data is split into train and test data set in the ratio 80:20.

### K-Nearest Neighbour
The K-nearest neighbours (KNN) algorithm is a type of supervised machine learning algorithms. KNN is extremely easy to implement in its most basic form, and yet performs quite complex classification tasks. Here KNN is implemented with Python's Scikit-Learn library.
f1 score: 0.6720916706047082 Accuracy score: 0.67088

### Decision Trees
Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features.
f1 score: 0.67519080668298 Accuracy score: 0.6754

### Logistic Regression
Logistic regression is a fundamental classification technique. It belongs to the group of linear classifiers and is somewhat similar to polynomial and linear regression. Logistic regression is fast and relatively uncomplicated, and it’s convenient for you to interpret the results. Although it’s essentially a method for binary classification, here it is applied to multi-class problems as one verses other method.
f1 score: 0.6720916706047082 Accuracy score: 0.6774341492949696

### Support Vector Machine (SVM)
Support vector machines (SVMs) are a set of supervised learning methods used for classification, regression and outliers detection. The advantages of support vector machines are Effective in high dimensional spaces, Still effective in cases where number of dimensions is greater than the number of samples, Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient, Versatile: different Kernel functions can be specified for the decision function.
f1 score: 0.6774341492949696 Accuracy_score: 0.67319

## Conclusions
In this study, I analyzed the relationship between various features and Traffic Accident Severity. Here classification models is used to predict Traffic Accident Severity. These models can be very useful effective in management of accident, mitigating accident impacts and improvingtrafficsafetyaccidentsandthustheenhancementofroadsafety. Itisamajor concern to societies due to the losses in human lives and the economic and social costs. It could help identify the severity and it help to improve road transportation system efficiency.
## Future directions
I was able to achieve 67% of accuracy in the classification problem. However, there was still significant variance that could not be predicted by the models in this study. I think the models could use more improvements on capturing date of incident, month, weekend or not, place, street, etc. And here only 15% of total dataset is used due to computational problems. More data, especially data of different types, would help improve model performances significantly.


[Report](https://github.com/AbhinandGK/Prediction-for-Traffic-Accident-Severity/blob/master/Project_report.pdf)
[Presentation](https://github.com/AbhinandGK/Prediction-for-Traffic-Accident-Severity/blob/master/presentation.pptx)
[ipynb](https://github.com/AbhinandGK/Prediction-for-Traffic-Accident-Severity/blob/master/accident_severity.ipynb)
