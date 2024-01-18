# Spatial Prediction of Socio-Economic Effects on Schedule Overrun Occurrences of Roadway Projects using Machine Learning Techniques
- A prediction model to measure and visually represent the effects of socioeconomic factors on the schedule overrun occurrences (SOO) of road projects

 *  Copyright (C) 2024  The University of Texas at Arlington
 *  Copyright (C) 2024  HBE: The Humanized Built Environment, (https://hubilab.uta.edu/)
 *  Copyright (C) 2024  Alireza Shamshiri, Kyeong Rok Ryu, Steven McCullough, and June Young Park

## Data Collection and Integration 
This project involves the analysis of integrated data from various sources spanning the years 2018 to 2020 across the State of Florida. The analyzed data included the following attributes:
(Integration of geospatial data was conducted using ArcGIS)

<p align="center">
		<img align="left" src="https://github.com/Alireza-shm/CatBoost_SOO_Prediction/blob/main/Images/Data.png" "height="200" width="200" />
</p>

 * Project-specific Factors
 * Transportation Data
 * socio-economic Factors
 * macroeconomic Factors
 * Weather Data



## Model Development and Selection
This project utilized several classifiers including `XGBoost`, `CatBoost`, `LightGBM`, `Random Forest`, `Logistic Regression`

|       Metric      | F1 | Precision | Recall | Training Accuracy | Testing Accuracy | ROC AUC |
|-------------------|----|-----------|--------|-------------------|------------------|---------|
|`Improved CatBoost`|94% |91%|98%|90%|89%|84%|
