# H1N1-vaccine-prediction-model
## Project Overview

The H1N1 vaccination prediction model is a machine learning project aimed at forecasting the demand for H1N1 influenza vaccinations. It utilizes historical vaccination data, demographic information, epidemiological factors, and possibly other relevant variables to predict the likely uptake of H1N1 vaccinations within a given population. 

The model's predictions can aid healthcare authorities and policymakers in planning vaccination campaigns, allocating resources effectively, and promoting public health initiatives to combat the spread of the virus.

## Methodology

In our quest for the most accurate model in predicting H1N1 vaccination demand, we adopted a multifaceted approach. Recognizing the complexity of model optimization due to various hyperparameters, we employed GridSearchCV to identify optimal combinations for each model. To counter the challenge posed by class imbalance, we prioritized balanced class weights whenever feasible. Our evaluation criteria encompassed accuracy, precision, F1 score, and ROC-AUC curve analysis for each model. Through meticulous comparison of ROC-AUC curves, we discerned the model with the most promising performance. Additionally, a thorough examination of the confusion matrix guided our focus on minimizing false positives. After comprehensive scrutiny, the Gradient Boosting Classifier emerged as the standout performer, excelling in accuracy and precision scores, thus earning its designation as our final model.

## Project Results

Among all models assessed, the Gradient Boosting model emerges as the frontrunner, boasting the highest aggregate scores and effectively minimizing false positives. Crucially, it demonstrates robust generalization, exhibiting comparable performance metrics—AUC, precision, and accuracy—across both the training and holdout datasets. This consistency instills confidence in its ability to extrapolate to unseen data, empowering public health officials with accurate insights into vaccination non-compliance.

Moreover, delving into feature importances elucidates the nuanced dynamics between predictors and vaccination behavior. Surprisingly, demographic and behavioral attributes pale in significance compared to health-related factors and opinions. Notably, factors such as doctor recommendations, possession of health insurance, perceived vaccine efficacy, and perception of H1N1 risk emerge as pivotal influencers in shaping individuals' vaccination status.
