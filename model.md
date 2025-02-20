# Personalised Learning Prediction Model Documentation

## Model Description

**Input:** The model takes in student-related features such as:
* Age
* Study hours
* Previous scores
* Engagement level
* Parental involvement
* Attendance percentage
* Self-motivation
* Categorical variables (Gender, Learning Resources, Learning Style) encoded using One-Hot Encoding

**Output:** The model predicts the final score of a student based on the given input features.

**Model Architecture:** The model is built using multiple regression-based architectures, including:
* Random Forest Regressor (Optimised via GridSearchCV)
* Gradient Boosting Regressor (Optimised via GridSearchCV)
* Multi-Layer Perceptron (Neural Network) with optimised hyperparameters

## Performance

The model's performance is evaluated using the following metrics:
* Mean Absolute Error (MAE)
* R² Score

Performance comparison:
* **Random Forest:** Best MAE: 3.85, R²: 0.76
* **Gradient Boosting:** Best MAE: 4.10, R²: 0.72
* **Neural Network:** Best MAE: 9.50, R²: -0.30

Visualisation of R² scores across models shows that Random Forest performs best.

## Limitations

* The model is trained on a specific dataset and may not generalise well to students with different learning environments.
* The dataset does not include external influences such as psychological factors, socioeconomic status, or unexpected events affecting student performance.
* Neural Network performance is significantly weaker, possibly due to the dataset size or lack of extensive tuning.

## Trade-offs

* **Complexity vs. Interpretability:** Random Forest and Gradient Boosting models perform well, but they are harder to interpret compared to simpler linear regression models.
* **Training Time:** Neural Networks require more computational resources and training time compared to tree-based models.
* **Bias and Fairness:** The dataset should be checked for potential biases related to gender, learning styles, or access to resources before deploying the model in real-world applications.
