# Spatial Prediction of Socio-Economic Effects on Schedule Overrun Occurrences of Roadway Projects using Machine Learning Techniques
- A prediction model to measure and visually represent the effects of socioeconomic factors on the schedule overrun occurrences (SOO) of road projects

 *  Copyright (C) 2024  The University of Texas at Arlington
 *  Copyright (C) 2024  HBE: The Humanized Built Environment, (https://hubilab.uta.edu/)
 *  Copyright (C) 2024  Alireza Shamshiri, Kyeong Rok Ryu, Steven McCullough, and June Young Park

## Data Collection and Integration 
This project involves the analysis of integrated data from various sources spanning the years 2018 to 2020 across the State of Florida. The analyzed data included the following attributes:
(Integration of geospatial data was conducted using ArcGIS)
(288 projects - 70 features)

 * Project-specific Factors
 * Transportation Data
 * socio-economic Factors
 * macroeconomic Factors
 * Weather Data

## Model Development and Selection
 * This project utilized several classifiers including `XGBoost` `CatBoost` `LightGBM` `Random Forest` and `Logistic Regression`
 * This project improved a `CatBoost` using top ten features with the following `performance`

|       Metric      | F1 | Precision | Recall | Training Accuracy | Testing Accuracy | ROC AUC |
|-------------------|----|-----------|--------|-------------------|------------------|---------|
|`Improved CatBoost`|94% |91%|98%|90%|89%|84%|

## Analysis

This project utilized `SHAP` values and plots to better intrepret the results of the `improved catboost` classifier.
<p align="center">
		<img align="center" src="https://github.com/Alireza-shm/CatBoost_SOO_Prediction/blob/main/Images/Analysis.png" "height="700" width="1000" />
</p>

## Spatial Mapping and Results Using Arc Geographic Information System (GIS)
The prediction results are plotted on the map of Florida by extracting `SHAP` values and importing into the Online ArcGIS which is accessible :

<p align="center">
		<img align="center" src="https://github.com/Alireza-shm/CatBoost_SOO_Prediction/blob/main/Images/Result.png" "height="100" width="100" />
</p>
