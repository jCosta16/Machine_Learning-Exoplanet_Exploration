# Machine Learning - Exoplanet Exploration

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I applied 3 machine learning models, capable of classifying candidate exoplanets from the raw dataset. For that purpose I followed theses steps:



1. [Preprocess the raw data]
2. [Tune the models Parameters]
3. [Compare two or more models]

Below you can find a report with a comparison of 3 model's performance as well as a summary about my findings and assumptions based on the model with the best performance.

## Summary
On the initially I used 31 of the 41 features (columns whit data), and used ```GrindSearch``` tunning the models to get a better result. 
For Them I selected the 21 most relevant features to run all the models again. This top 21 where pickup by using ```feature_importances_``` as the selection method.

***

## Conclusion
With the Hypertuning of the ```GrindSearch```  the SVC model achieves a better accuracy then the Random Forest model. 
However reducing the number of features the Ramdon Forest model has a better performance.

We can also notice that, even redducing the number of features in 30% the accuracy for every models dos not have a significant drop in performance. 



## **SVC**

|  Clean Data    | Before GrindSearch | After GrindSearch |
| -------------- |:------------------:| :----------------:|
| Training Score |        0.83342     |      0.87521      |
| Testing Score  |        0.83638     |      0.89054      |

| TOP21 Features | Before GrindSearch | After GrindSearch |
| -------------- |:------------------:| :----------------:|
| Training Score |        0.79851     |      0.87464      |
| Testing Score  |        0.80377     |      0.88291      |


## **Deep Learning**

|  Clean Data    | 100 eopochs |
| -------------- |:-----------:|
| Loss           |   0.31877   |
| Accuracy       |   0.86594   |

| TOP21 Features | 100 eopochs |
| -------------- |:-----------:|
| Loss           |   0.36154   |
| Accuracy       |   0.84591   |


## **Random Forest**

|  Clean Data    | Before GrindSearch | After GrindSearch |
| -------------- |:------------------:| :----------------:|
| Training Score |        0.99427     |      1.0          |
| Testing Score  |        0.86861     |      0.88920      |

| TOP21 Features | Before GrindSearch | After GrindSearch |
| -------------- |:------------------:| :----------------:|
| Training Score |        0.99484     |      1.0          |
| Testing Score  |        0.85354     |      0.88367      |


***
