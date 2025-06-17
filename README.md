
## Project Overview

Research Question:
"How effectively can a combination of meteorological attributes, atmospheric conditions, and visibility factors predict weather type, and which features play the most significant role in distinguishing between different weather categories?"

Objective:
The objective of this study is to build a classification model that predicts the weather type using a combination of meteorological, atmospheric, and environmental attributes. By identifying the most influential features, this research aims to enhance the understanding of weather patterns, improve forecasting accuracy, and aid decision-making in weather-dependent domains such as agriculture, transportation, and disaster management.

## Dependant and Independant Variables 
Target Variable:
Weather Type - This variable categorizes weather conditions into specific types, serving as the classification target for our model.

Features:
The dataset includes 14 predictive attributes categorized into four main groups, which will be utilized to predict the weather type.

Meteorological Attributes:

Temperature: Represents the atmospheric temperature in degrees Celsius.
Humidity: Measures the amount of water vapor in the atmosphere, expressed as a percentage.
Wind Speed: Indicates the speed of the wind in kilometers per hour (km/h).
Precipitation (%): Reflects the likelihood of precipitation as a percentage.
Cloud Cover: Represents the fraction of the sky obscured by clouds.

Atmospheric Conditions:

Atmospheric Pressure: Measures the pressure exerted by the atmosphere, typically in millibars.
UV Index: Indicates the level of ultraviolet radiation on a given day, on a scale from 0 (low) to 11+ (extreme).

Environmental and Visibility Factors:

Season:A categorical variable representing the season during which the data was recorded.
Visibility (km): Measures the horizontal distance at which objects can be clearly seen.
Location: Denotes the geographical area where the data was collected.

Derived and Related Metrics:

Heat Index: A derived metric indicating how hot it feels when accounting for both temperature and humidity.
Precipitation Intensity: Represents the intensity of precipitation during the recorded period.

Excluded Variables:

Dew Point: A metric indicating the temperature at which air becomes saturated with moisture, excluded due to redundancy.
Wind Chill: The perceived decrease in air temperature due to wind, excluded for its lack of direct predictive value for weather type classification.

## Conclusions and models used
After hyperparameter tuning, the results show improved model performance, with significant variations across different algorithms.

Logistic Regression achieved a training accuracy of 0.893 and a test accuracy of 0.905, which indicates a good fit to the data with minimal overfitting. The relatively small gap between training and test accuracy suggests the model generalizes well.

K-Nearest Neighbors (KNN) showed training accuracy of 0.930 and test accuracy of 0.918, demonstrating a solid performance with a small difference between training and test accuracies, indicating it is a reliable model that generalizes well.

Naive Bayes had training accuracy of 0.813 and test accuracy of 0.818, suggesting that despite hyperparameter tuning, it is still underperforming compared to other models. However, it does maintain a close match between training and test accuracy, implying it is not overfitting but just less effective at capturing the complexity of the data.

Gradient Boosting demonstrated excellent performance, with a training accuracy of 0.963 and test accuracy of 0.944, indicating that the model is highly effective with a very small drop in performance from training to test data, showing that it has been tuned for optimal performance and generalizes well.

Random Forest achieved training accuracy of 1.000 and test accuracy of 0.950, suggesting potential overfitting, as the model perfectly fits the training data. However, the high test accuracy indicates that it is still able to generalize effectively, even if overfitting is a concern.

Decision Tree showed training accuracy of 1.000 and test accuracy of 0.945, similar to Random Forest. The perfect training accuracy indicates overfitting, but it still performs well on the test data, though tuning may be required to reduce overfitting further.

Support Vector Machine (SVM) recorded training accuracy of 0.909 and test accuracy of 0.922, with a relatively small gap between the two, indicating a well-balanced model that generalizes well after hyperparameter tuning.

In conclusion, Gradient Boosting continues to be the best performer, with a minimal gap between training and test accuracies. Random Forest and Decision Tree show potential overfitting due to the perfect training accuracy, but they still perform well on the test set. KNN and Logistic Regression provide solid and reliable performance, while Naive Bayes remains the weakest performer, even after hyperparameter tuning.

## Key Features

Product-wise Analysis – Compare sales and pricing across different shoe models

Price Distribution – Visualize price ranges using histograms/bar charts

Sales Insights – Track best-selling products and revenue trends

Interactive Filters – Filter data by product, price range, sales volume, and time
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
