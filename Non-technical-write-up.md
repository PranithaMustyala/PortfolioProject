# **Personalised Learning Performance Prediction**

## **Overview**
Education is not one-size-fits-all. Every student has unique learning styles, study habits, and external influences that impact their academic performance. This project aims to predict students' final scores based on key factors such as engagement level, study hours, previous scores, and learning styles. By analysing these patterns, educators and students can gain insights into how different elements contribute to academic success.

## **Objective**
The goal of this project is to develop a machine learning model that can predict a student's final score based on various input features. This model can help:
* **Educators** identify students who may need additional support.
* **Students** understand which habits lead to better academic performance.
* **Institutions** develop personalised learning strategies.

## **How It Works**
We use a dataset containing student-related factors, including demographic information, study habits, attendance, and engagement levels. The data is processed by:
* **Encoding categorical variables** like gender and learning style.
* **Normalising numerical features** such as study hours and previous scores.
* **Splitting the data** into training and testing sets.

We then train multiple machine learning models to determine which provides the most accurate predictions. The models tested include:
1. **Random Forest Regressor** – A tree-based model that captures complex patterns in student performance.
2. **Gradient Boosting Regressor** – A boosting algorithm that improves predictions over multiple iterations.
3. **Neural Network (MLP Regressor)** – A deep learning approach to understand nonlinear relationships in the data.

## **Key Findings**
* The **Random Forest model** performed best, with a strong predictive accuracy (**R² = 0.76, MAE = 3.85**).
* The **Gradient Boosting model** followed closely, though slightly less accurate.
* The **Neural Network model** underperformed, likely due to the dataset size and the nature of the data.

## **Impact and Future Scope**
This project highlights the power of machine learning in education. By analysing key performance indicators, we can develop tailored interventions to support student success. Future improvements could include:
* Collecting additional features such as psychological and environmental factors.
* Exploring deep learning models with larger datasets.
* Implementing an interactive tool for educators to visualise predictions.

By leveraging data-driven insights, we can enhance personalised learning experiences and improve educational outcomes for students worldwide.
