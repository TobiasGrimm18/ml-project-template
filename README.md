# [Predicting Bakery Sales using linear regression and neural nets Group 1]

## Repositor Link

[https://github.com/mofreund99/TeamCPH.git]

## Description
- Revenue forecasting project for bakery product groups using daily sales plus external signals (weather and event/calendar effects), comparing a simple linear baseline to an MLP neural network.

**Task Type**
- Regression

**Results Summary**
- Best Model: Neural Net (MLP)
- Evaluation Metric: RMSE (primary for cross-model comparison), with MAE/MAPE as supporting metrics
- Best Model Performance: MAE 36.62, RMSE 63.64, MSE 4049.52, Validation MAPE 24.60%

**Model Comparison**
- Baseline Performance: MAE 105.10, RMSE 147.10, MAPE 63.83%, R² (log-space) 0.0373
- Improvement Over Baseline: MAE improved by 65.2%, RMSE improved by 56.7%, MSE improved by 81.3%

**Key Insights**
- Most Important Features: Revenue_lag1, Revenue_lag7, IsWeekend, KielerWoche, Temperatur
- Model Strengths: Captures nonlinear feature interactions; substantially lowers forecast error vs baseline
- Model Limitations: Less interpretable than linear models; sensitive to split consistency and scaling; MAPE can be unstable near zero true values
- Business Impact: Better forecasts improve staffing, procurement, and event-day production planning while reducing costly over/under-production decisions

## Documentation

1. **[Literature Review](0_LiteratureReview)**
2. **[Dataset Characteristics](1_DatasetCharacteristics/exploratory_data_analysis_Team1.ipynb)**
3. **[Baseline Model](2_BaselineModel)**
4. **[Model Definition and Evaluation](https://github.com/TobiasGrimm18/ml-project-template/blob/c22d60abe75b14558b83dfb9690b1f14b5d84a32/3_Model/model_definition_evaluation%20(3).ipynb)**
5. **[Presentation](4_Presentation)**

## Cover Image

![Project Cover Image](https://github.com/TobiasGrimm18/ml-project-template/blob/6d6cc514746ac6a2fbb9bc49502a6f042c04b1ec/CoverImage/Coverimage.png)
