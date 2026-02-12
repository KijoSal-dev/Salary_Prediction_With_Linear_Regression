# Salary_Prediction_With_Linear_Regression
This project demonstrates how to build a simple linear regression model to predict salaries based on experience, test scores, and interview scores. The process includes data preprocessing, model training, and prediction.

## What I Did

1.  **Data Loading**: Loaded a CSV file named `hiring (1).csv` into a Pandas DataFrame.
2.  **Data Preprocessing**:
    *   Converted the 'experience' column from word format (e.g., 'five') to numerical format (e.g., 5) using a custom mapping.
    *   Handled missing values in the 'experience' and 'test_score(out of 10)' columns by imputing them with their respective median values.
3.  **Model Training**: Implemented a Linear Regression model from `sklearn.linear_model`.
    *   Defined features (X) as 'experience', 'test_score(out of 10)', and 'interview_score(out of 10)'.
    *   Defined the target variable (y) as 'salary($)'.
    *   Trained the linear regression model using the preprocessed data.
4.  **Prediction**: Used the trained model to predict salaries for two new hypothetical candidates.
5.  **Visualization**: Plotted the original salary data against experience and overlaid the predicted salaries for the new candidates to visually assess the model's output.

## Why I Did It

The primary goal of this project was to understand and apply fundamental machine learning concepts, specifically linear regression, for a practical prediction task. This included:

*   Gaining experience with data preprocessing techniques, such as handling categorical data and missing values.
*   Learning to build and train a linear regression model using scikit-learn.
*   Interpreting model coefficients and making predictions.
*   Visualizing model predictions and comparing them with original data trends.

## Outcome

The linear regression model was successfully trained and was able to predict salaries for new candidates. The predictions were:

*   Candidate 1 (2 years experience, 9 test score, 6 interview score): **$47,056.91**
*   Candidate 2 (12 years experience, 10 test score, 10 interview score): **$88,227.64**

The visualization confirmed that the predicted salaries align well with the general trend in the dataset, where higher experience and scores generally correlate with higher salaries.

## Challenges Encountered

*   **Categorical to Numerical Conversion**: Converting the 'experience' column from descriptive words to numerical values required careful mapping to ensure data integrity.
*   **Missing Data Imputation**: Deciding on an appropriate imputation strategy (median imputation in this case) for missing 'experience' and 'test_score' values was crucial to avoid biased model training.
*   **Feature Engineering/Selection**: For a more complex scenario, determining the most impactful features for salary prediction would involve more rigorous feature engineering and selection techniques. For this project, existing relevant features were directly used.
