# Credit Risk Prediction

## Introduction
This project aims to develop a statistical model for predicting the likelihood of a borrower defaulting on a loan. The model utilizes relevant borrower data such as credit history, income, employment status, and demographic information to make predictions. By analyzing these features, the goal is to build a robust model that can accurately classify borrowers as either 'ok' or 'default'.

## Data Source
The dataset used in this project is sourced from [this link](https://github.com/gastonstat/CreditScoring/raw/master/CreditScoring.csv). It contains information about borrowers including their credit history, income, employment status, and loan default status.

## Approaches
- The project begins by importing the dataset and performing initial data preprocessing steps. This includes cleaning the data, handling missing values, and encoding categorical variables to ensure uniformity and consistency in the data.

- Exploratory data analysis is conducted to gain insights into the dataset and understand the distribution of borrower features. Visualizations such as histograms and heatmaps are utilized to analyze the relationships between different variables and identify any potential patterns or trends.

- To the model building, several machine learning models are built and evaluated to predict borrower default risk:
  **Decision Tree Classifier:** A decision tree classifier is trained using the borrower features to predict the likelihood of default. The model's performance is evaluated using the area under the ROC curve (AUC).
  **Random Forest Classifier:** A random forest classifier is trained using an ensemble of decision trees to improve prediction accuracy. The number of estimators and maximum depth of the trees are tuned to optimize performance.
  **XGBoost Classifier:** An XGBoost classifier is trained using gradient boosting techniques to further enhance prediction accuracy. Hyperparameters such as learning rate, maximum depth, and minimum child weight are tuned to optimize model performance.
**XGBoost Classifier Model** is the better model as it generalized better and showed improved performance.

- The trained models are evaluated using a validation dataset to assess their performance in predicting borrower default risk. Evaluation metrics such as AUC are used to quantify the models' accuracy and compare their performance.

## Conclusion
This project demonstrates the process of building machine learning models for credit risk prediction. By leveraging borrower data and utilizing advanced modeling techniques, accurate predictions can be made regarding the likelihood of loan default. Further optimizations and refinements can be explored to improve the models' performance and reliability.

## Deployment
The final XGBoost model is saved using BentoML for deployment and integration into production systems. This allows the model to be easily accessed and used for real-time credit risk prediction.
