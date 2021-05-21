# Road-Accident-Severity-Prediction 🚔🚨🚘
## Objective
The objective of this project was to focus on analyzing the factors which could help predict the severity of the accident. The results of analysis could be utilized by the Department of transport for safe route planning, Emergency Vehicle allocation, Roadway design and utilized by Google maps for better route recommendation to the users. 

## Dataset Information 
The data come from the Open Data website of the UK government, where they have been published by the Department of Transport.

The dataset comprises of two csv files:

1. AccidentInformation.csv: every line in the file represents a unique traffic accident (identified by the AccidentIndex column), featuring various properties related to the accident as columns. Date range: 2005-2017

2. Vehicle_Information.csv: every line in the file represents the involvement of a unique vehicle in a unique traffic accident, featuring various vehicle and passenger properties as columns. Date range: 2004-2016
The two above-mentioned files/datasets can be linked through the unique traffic accident identifier (Accident_Index column).

The dataset will keep being updated as more data become available by the Department of Transport.

## Requirements 

### Libraries are required as follows

* `numpy`
* `pandas`
* `matplotlib`
* `seaborn`
* `datetime`
* `geopandas` 
* `scikit-learn`

## Results

* We started our analysis with exploratory data analysis to discern the dataset. Machine learning algorithms were used to explore the complex interactions among roadways, traffic, environmental elements and predicting accident severity. Since most of the predictor variables in the dataset were categorical, we recoded categorical variables. 11 models were built, evaluated for complexity and accuracy, and compared to conclude which model is the best fit for predicting accident severity. 

* Spot Checking technique was used to fit the 11 models to determine which models would predict the accident severity with the highest accuracy. We also performed feature engineering to enrich our dataset Hyperparameter tuning and pipelining the best performing model helped to improve the performance of the model by making accurate predictions. Gradient Boosting performed well with the accuracy of 86.71% and which were further improved by doing permutation testing for feature importance which played an important role in predictions.

```
Logistic Regression_1
56.33
Random Forest_1
60.52
Gradient Boosting_1
86.71
Linear Discriminant Analysis_1
55.76
Extra Trees_1
58.62
Bagging_1
55.67
```

#### Gradient Boosting scores
```
Model	Score
0	Gradient Boosting_1	86.71
```

#### Conclusion
Among all other techniques used, Gradient Boosting Classifier has performed best with the highest accuracy. One reason why RF works well is because the algorithm can look past and handle the missing values in the tweets.

#### Project Contributer
Lei Cao 
