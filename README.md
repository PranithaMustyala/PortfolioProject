# Personalised Learning Performance Prediction

This project aims to predict students' final scores based on factors such as engagement, study habits, and learning styles. By analysing these variables, the model helps educators and students understand which factors contribute most to academic success, enabling personalised learning recommendations.

## Data
The dataset contains student-related features, including age, study hours, previous scores, engagement levels, and learning styles. It was sourced from educational research and anonymised student records. Categorical features were encoded, and numerical data was normalised to improve model performance.

## Model
Three models were trained and evaluated:
* **Random Forest Regressor**: Chosen for its ability to handle complex relationships in data.
* **Gradient Boosting Regressor**: Selected for its strong performance on structured data.
* **Neural Network (MLP Regressor)**: Explored to test deep learning capabilities in this context.

Random Forest performed the best in terms of accuracy and error minimisation.

## Hyperparameter Optimisation
Hyperparameters were optimised using `GridSearchCV` to improve model performance. Key optimisations included:
* Number of estimators for Random Forest and Gradient Boosting
* Learning rate for Gradient Boosting
* Hidden layer sizes and activation functions for the Neural Network

## Results
* **Random Forest:** MAE: 3.85, R²: 0.76
* **Gradient Boosting:** MAE: 4.10, R²: 0.72
* **Neural Network:** MAE: 9.50, R²: -0.30

The Random Forest model provided the best balance of performance and interpretability.
