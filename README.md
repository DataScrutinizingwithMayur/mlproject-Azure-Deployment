## End-to-End Machine Learning project
# Student Performance Analysis Project

## Overview
This project analyzes and predicts student performance based on factors such as gender, ethnicity, parental education, lunch type, and test preparation course. The aim is to understand and quantify the impact of these factors on students' academic performance specifically to predict the Math score based on all the dependent variables.

## Data Source
The data for this project is sourced from the "Students Performance in Exams" dataset available on Kaggle. It comprises 1000 entries with 8 columns representing different attributes related to student demographics and academic performance.

## Methodology
The project is structured into two main parts:

1. **Exploratory Data Analysis (EDA)**
   - Analysis of the data to understand trends and patterns.
   - Identification of key factors that significantly impact student performance.

2. **Model Training and Evaluation**
   - Development of machine learning models to predict student performance.
   - Used various regression models like KNN, Decision Tree, Random Forest, AdaBoost, SVR, Linear Regression, Ridge, Lasso, CatBoost, and XGBoost.
   - Evaluation of models using metrics such as R2 score, mean absolute error and mean squared error.

## Key Findings
   - Student performance is influenced by factors like lunch type, race, and parental education level.
   - Female students tend to have a higher pass percentage and are often top-scorers.
   - There isn't a strong relationship between student performance and the completion of a test preparation course.
   - Completing a preparation course is beneficial, albeit not a primary factor in academic success.
   - Based on all the models that are used for this regression task, the linear regression model stands out with an R2 score of 87.90 on the test data set.

## Technologies Used
- Python
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, CatBoost, XGBoost


Certainly! Here's a "How to Use" section for your README.md file, which details how users can interact with your deployed model on AWS Elastic Beanstalk through the Flask web application:

markdown
Copy code
## How to Use

### Accessing the Web Application
The machine learning model for predicting student performance has been deployed as a web application. You can access it using the following link:

[Student Performance Predictor](http://studentperformance-env-1.eba-eu8qbkh8.us-east-2.elasticbeanstalk.com/predictdata)

### Making Predictions
1. **Open the Web Application**: Use the provided link to navigate to the application.
2. **Input Data**: Enter the required data related to student demographics and academic background. The input fields correspond to the features used by the machine learning model.
3. **Submit for Prediction**: After filling in the data, submit it to receive the performance prediction. The model will process the input and display the predicted performance.

### Behind the Scenes
- **Deployment**: The application is deployed on AWS Elastic Beanstalk, ensuring scalability and reliability.
- **Continuous Integration/Continuous Deployment (CI/CD)**: The project uses AWS CodePipeline for automating the deployment process. Any updates to the GitHub repository trigger a new deployment cycle, ensuring the application is always up-to-date.
- **Technology Stack**: 
  - **Backend**: The backend is built using Flask, a lightweight and efficient web framework in Python, ideal for creating RESTful APIs.
  - **Model Hosting**: The machine learning model is hosted on AWS, allowing for efficient handling of web requests and model predictions.

