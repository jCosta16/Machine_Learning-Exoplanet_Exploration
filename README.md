# Machine Learning - Exoplanet Exploration


## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I createed 2 machine learning models, capable of classifying candidate exoplanets from the raw dataset. For that purpose I followed theses steps:

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

Below you can find a report with a comparison of two model's performance as well as a summary about my findings and assumptions based on the model with the best performance.



#### Conclusion
With very little training the neural achieves the same accuracy as the SVM model. However with the Hypertuning the SVM model achieves significantly higher accuracy of 88% which surpasses the Neural Network. It would be interesting to see if/how-many epochs of the neural network it would take to achieve the same accuracy.

