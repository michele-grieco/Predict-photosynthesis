# Predicting Photosynthesis with Ensemble Models and Neural Networks

## Overview
This project focuses on predicting the photosynthesis rate, measured as Linear Electron Flow (LEF), in barley plants. The data was collected from a field experiment involving 127 genotypes, conducted in 2017 at the Leibniz Institute of Plant Genetics and Crop Plant Research (IPK) in Germany. This analysis is aimed at identifying key factors influencing photosynthesis and developing predictive models to estimate LEF under field conditions.

## Dataset
The dataset includes various features such as:
- Genotype
- Time of Day
- Light Intensity
- Ambient Humidity
- Ambient Temperature
- SPAD Measurements (SPAD_650, SPAD_880)
- LEF (target variable)

Data preprocessing included normalization, manual feature selection, and determination of feature importance using Random Forest.
Data are not available here because not yet published in a peer-reviewed journal.

## Models and Methodology
Several ensemble models were employed to predict LEF:
- **Random Forest**
- **LightGBM**
- **XGBoost**
- **CatBoost**

In addition, Neural Networks were trained and optimized using Keras.

Feature importance was determined using Random Forest, and the most significant features were selected for model training. Hyperparameter tuning was performed using `RandomizedSearchCV` to optimize model performance.


## Results

The performance of various models in predicting Linear Electron Flow (LEF) was evaluated using metrics such as Root Mean Squared Error (RMSE), Mean Absolute Percentage Error (MAPE), and Mean Absolute Error (MAE)). The table below summarizes the results:

| Model         | RMSE      | MAPE      | MAE       |
|---------------|-----------|-----------|-----------|
| RandomForest  | 12.301    | 0.069     | 8.250     |
| XGBoost       | 12.389    | 0.070     | 8.180     |
| LightGBM      | 12.308    | 0.073     | 8.221     |
| CatBoost      | 12.226    | 0.077     | 8.291     |
| Neural Network| 17.138    | 0.148     | 13.374    |



## Acknowledgments

I thank the IPK Institute and the PhotosynQ team for their support.


