### Exploratory Data Analysis and Model Evaluation for Salary Prediction

This code snippet demonstrates the process of building and evaluating a simple linear regression model for predicting salaries based on years of experience. It involves several key steps:

1. **Data Preprocessing:**
   - The code begins by importing necessary libraries and loading the dataset from a CSV file (`Salary_Data.csv`).
   - It separates the independent variable (years of experience, `X`) and dependent variable (salary, `y`).
   - Missing values in the independent variable are handled using mean imputation.
   - Categorical data (if any) is encoded using one-hot encoding for better model compatibility.
   - Label encoding is applied to the dependent variable if it contains categorical values.

2. **Data Splitting:**
   - The dataset is split into training and testing sets using a 80-20 ratio. This allows for model training and evaluation on independent datasets.

3. **Feature Scaling:**
   - Standard scaling is performed on the independent variables to ensure all features contribute equally to the model fitting process.

4. **Model Training:**
   - A linear regression model is instantiated and trained using the training data.

5. **Model Visualization:**
   - The code generates two scatter plots:
     - One showing the actual vs. predicted salaries on the training set to visualize how well the model fits the training data.
     - Another showing the actual vs. predicted salaries on the test set to evaluate model performance on unseen data.

6. **Model Evaluation:**
   - Mean Squared Error (MSE) and R-squared (R²) are computed to quantify the performance of the regression model on the test set. These metrics provide insights into the accuracy and goodness of fit of the model.

The scatter plots help visualize how well the model captures the relationship between years of experience and salary, while the evaluation metrics provide quantitative measures of model performance. This process is essential for understanding the effectiveness of the regression model in predicting salaries based on experience.
