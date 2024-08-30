**Problem Statement:**

You are a data scientist at a telecom company named "Neo" that is experiencing customer churn, where customers are leaving for competitors. Your task is to analyze the company's data to uncover insights and develop strategies to prevent further customer churn.

**Dataset:**
The dataset provided is titled 'customer_churn'. A detailed data dictionary accompanies this dataset.

**Environment:**
Lab Environment: Anaconda  
Domain: Telecom

**Tasks to be Performed:**

1. **Data Manipulation:**
   - Extract the 5th column and store it in a variable named `customer_5`.
   - Extract the 15th column and store it in a variable named `customer_15`.
   - Identify all male senior citizens who use electronic check as their payment method and store them in `senior_male_electronic`.
   - Extract all customers whose tenure exceeds 70 months or whose monthly charges are over $100, and store them in `customer_total_tenure`.
   - Identify all customers who have a two-year contract, use mailed check as their payment method, and have a churn status of 'Yes'. Store these records in `two_mail_yes`.
   - Randomly select 333 records from the `customer_churn` dataset and store them in `customer_333`.
   - Count the different levels present in the 'Churn' column.

2. **Data Visualization:**
   - **Bar Plot for `InternetService` column:**
     - Set the x-axis label to ‘Categories of Internet Service’.
     - Set the y-axis label to ‘Count of Categories’.
     - Title the plot as ‘Distribution of Internet Service’.
     - Set the bar color to 'orange'.
   - **Histogram for `tenure` column:**
     - Set the number of bins to 30.
     - Set the bin color to ‘green’.
     - Title the histogram ‘Distribution of tenure’.
   - **Scatter Plot between `MonthlyCharges` and `tenure`:**
     - Map `MonthlyCharges` to the y-axis and `tenure` to the x-axis.
     - Assign the points a color of ‘brown’.
     - Set the x-axis label to ‘Tenure of customer’.
     - Set the y-axis label to ‘Monthly Charges of customer’.
     - Title the plot ‘Tenure vs Monthly Charges’.
   - **Box Plot between `tenure` & `Contract`:**
     - Map `tenure` on the y-axis.
     - Map `Contract` on the x-axis.

3. **Linear Regression:**
   - Build a simple linear regression model where the dependent variable is `MonthlyCharges` and the independent variable is `tenure`:
     - Split the dataset into training and testing sets in a 70:30 ratio.
     - Train the model on the training set and predict values on the test set.
     - Calculate the root mean square error (RMSE) for the predictions.
     - Store the error in a variable named `error`.

4. **Logistic Regression:**
   - Build a simple logistic regression model where the dependent variable is `Churn` and the independent variable is `MonthlyCharges`:
     - Split the dataset into training and testing sets in a 65:35 ratio.
     - Train the model on the training set and predict values on the test set.
     - Build a confusion matrix and calculate the accuracy score.
   - Build a multiple logistic regression model where the dependent variable is `Churn` and the independent variables are `tenure` and `MonthlyCharges`:
     - Split the dataset into training and testing sets in an 80:20 ratio.
     - Train the model on the training set and predict values on the test set.
     - Build a confusion matrix and calculate the accuracy score.

5. **Decision Tree:**
   - Build a decision tree model where the dependent variable is `Churn` and the independent variable is `tenure`:
     - Split the dataset into training and testing sets in an 80:20 ratio.
     - Train the model on the training set and predict values on the test set.
     - Build a confusion matrix and calculate the accuracy score.

6. **Random Forest:**
   - Build a Random Forest model where the dependent variable is `Churn` and the independent variables are `tenure` and `MonthlyCharges`:
     - Split the dataset into training and testing sets in a 70:30 ratio.
     - Train the model on the training set and predict values on the test set.
     - Build a confusion matrix and calculate the accuracy score.
