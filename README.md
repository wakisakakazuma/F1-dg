# Machine Learning-Based Prediction Model for F1 Tire Degradation

## Abstract
#### This project uses machine learning to analyze and predict F1 tire degradation. We aim to build a machine learning model that helps optimize race strategy by analyzing and visualizing the time-dependent degradation of tires using data such as weather conditions, circuit characteristics, and car performance.

## Introduction
#### In Formula 1 and other forms of motorsport, understanding tire behavior is one of the most critical performance factors, as tire management and selection often determine a race's outcome. Accurately predicting tire degradation patterns is essential for formulating optimal race strategies. While F1 teams use various predictive methods, analogous tools are not readily available to fans. There are currently no public tools that provide systematic visualization or prediction of tire degradation. This study aims to fill this gap by developing a predictive model for tire degradation using publicly available race data. This framework aims to enhance enjoyment not only for new fans but also for core fans, amidst the recent growth in the fan base.

## Methodology
#### This project utilized race data from the 2024 Formula 1 season.The majority of the datasets were sourced from FastF1. Information concerning engine manufacturers used by each team was gathered from external sources, specifically https://rtrsports.com/, while track characteristics were compiled with reference to Formula1-Data.The classification for the track corners was defined based on vehicle speed as follows: high-speed corners were considered over 200 km/h, medium-speed corners were defined as 120 km/h to 200 km/h, and low-speed corners were categorized as under 120 km/h.To ensure the efficient processing of diverse features, a scikit-learn Pipeline was employed. This pipeline automated the necessary preprocessing steps, including the normalization of numerical features, ordinal encoding of tire compounds, and one-hot encoding of engine manufacturers.Tire degradation was predicted through the application of regression analysis using machine learning techniques.

## Evaluation
#### The model's performance evaluation was conducted on post-training data to verify its accuracy and reliability. Specifically, the model was assessed using two primary quantitative metrics—Mean Squared Error (MSE) and the Coefficient of Determination (R2) score—with the resulting high goodness-of-fit indicating that the model captured the actual tire degradation patterns with exceptional precision. Furthermore, Feature Importance analysis, extracted from the Random Forest Regressor, was utilized to identify the contribution of each input element to the prediction, thereby verifying that the model not only achieved high predictive accuracy but also made logical judgments based on underlying physical causality.

## References
#### RTR Sports Marketing. (2025, April 4). 2025 F1 Engine Specs. Retrieved from https://rtrsports.com/ja/2025%E5%B9%B4f1%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%B3%E3%82%B9%E3%83%9A%E3%83%83%E3%82%AF/

#### Formula1-Data. (n.d.). Circuit Guide. Retrieved from https://formula1-data.com/