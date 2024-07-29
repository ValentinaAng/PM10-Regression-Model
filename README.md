# Project Title: 
Center PM10 Regression

# Project Description:
This project involves the preprocessing, training, and evaluation of regression models on a dataset containing various features.
The primary objective is to predict a target variable using different regression algorithms and compare their performances.

# About Dataset:

| Feature            | Description                                                                                 |
|--------------------|---------------------------------------------------------------------------------------------|
| **apparentTemperature** | The apparent (“feels like”) temperature in degrees Fahrenheit.                           |
| **Cloud cover**        | The percentage of sky occluded by clouds.                                                 |
| **dewPoint**           | Temperature to which air must be cooled to become saturated with water vapor.              |
| **humidity**           | The relative humidity.                                                                      |
| **precipIntensity**    | The intensity (in inches of liquid water per hour) of precipitation.                       |
| **precipProbability**  | The probability of precipitation occurring.                                                |
| **pressure**          | The sea-level air pressure in millibars.                                                    |
| **temperature**       | The air temperature in degrees Fahrenheit.                                                  |
| **time**              | The UNIX time at which this data point begins.                                              |
| **Visibility**        | The average visibility in miles.                                                            |
| **windBearing**       | The direction that the wind is coming from in degrees with true north at 0° and progressing clockwise. |
| **windSpeed**         | The speed of the wind in miles per hour.                                                    |
| **PM10**              | (Target) Atmospheric particulate matter with a diameter smaller than 10 micrometers.        |
|**no_precip**          | precipitation is any product of the condensation of atmospheric water vapor that falls from clouds due to gravitational pull|
|**rain**| 0 - no, 1-yes|
| **sleet**|0 - no, 1-yes|
|**snow**| 0 - no, 1-yes|
|**clear**| 0 - no, 1-yes|
|**drizzle**| 0 - no, 1-yes|
|**foggy**| 0 - no, 1-yes|
|**mostly cloudy**| 0 - no, 1-yes|
|**overcast**| 0 - no, 1-yes|
|**partly cloudy**| 0 - no, 1-yes|

#Table of Contents:
1. Data Analysis
2. Data Cleaning
3. Exploratory Data Analysis
4. Data Preprocessing
5. Model Training and Hyperparameter Optimization
6. Model Evaluation
7. Results
8. Conclusion


# Results
### RandomForestRegressor as best model
- **R2 Score**: Train: 0.704, Test: 0.706
- **MAE**: Train: 24.369, Test: 25.116
- **RMSE**: Train: 40.372, Test: 41.505

### KNeighborsRegressor
- **R2 Score**: Train: 0.690, Test: 0.692
- **MAE**: Train: 22.354, Test: 24.298
- **RMSE**: Train: 41.282, Test: 42.487

### Conclusion
The RandomForestRegressor and KNeighborsRegressor both showed minimal signs of overfitting, with similar performance on both the training and test sets. 

### Recommendations for Improvement
- **Feature Engineering**: Explore additional feature engineering techniques.
- **Hyperparameter Tuning**: Further optimize hyperparameters using more exhaustive searches or advanced techniques like Bayesian Optimization.
- **Ensemble Methods**: Consider combining multiple models to form an ensemble for potentially better performance.
