# Machine Learning-Based Prediction Model for F1 Tire Degradation

## Abstract
#### This project uses machine learning to analyze and predict F1 tire degradation. We aim to build a machine learning model that helps optimize race strategy by analyzing and visualizing the time-dependent degradation of tires using data such as weather conditions, circuit characteristics, and car performance.

## Introduction
#### In F1 race strategy, tire degradation is a critical factor that can determine victory or defeat. However, there are currently no tools available for fans to predict and analyze this complex factor in real-time. This project aims to build a model that predicts degradation using publicly available race data, thereby enhancing the fun of watching F1 races.

## Definition
#### High-Speed Corners: Over 200 km/h
#### Medium-Speed Corners: 120 km/h to 200 km/h
#### Low-Speed Corners: Under 120 km/h

## Methodology
#### This project trained a model on 2024 season race data and validated its performance on specific race data. We used a scikit-learn pipeline to efficiently handle a wide range of features. This pipeline automatically performs preprocessing steps like numerical feature normalization, tire compound ordinal encoding, and engine manufacturer one-hot encoding. We chose RandomForestRegressor as our prediction model due to its ability to capture complex nonlinear relationships. By integrating the model with the preprocessing pipeline, we created a system that handles everything from data to prediction.

## Evaluation
#### The model's performance was evaluated using Mean Squared Error (MSE) and the Coefficient of Determination (R²). These metrics show how well our predicted values align with the actual degradation. We also analyzed the model's feature importance to identify each element's contribution to the prediction.