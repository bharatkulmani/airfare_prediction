# airfare_prediction
This Python project focuses on predicting flight ticket prices using a machine learning model. The dataset is loaded using pandas and then explored to understand its structure and content. Various preprocessing steps are performed to clean and transform the data into a suitable format for building the predictive model.

The main steps of the project are as follows:

Data Loading and Exploration:

The dataset is loaded from an Excel file ('Data_Train.xlsx') using pandas.
Basic information about the dataset, such as data types and missing values, is checked using methods like 'info()', 'describe()', 'isnull()', and 'any()'.
Rows with missing values are dropped from the dataset.
Feature Engineering:

The 'Date_of_Journey' column is converted to datetime format to extract the day and month of the journey.
The 'Dep_Time' and 'Arrival_Time' columns are also converted to datetime format to extract the hour and minute of departure and arrival times.
The 'Duration' column is preprocessed to convert the duration of flights from a string format (e.g., '2h 30m') to separate hours and minutes columns.
Data Transformation:

Categorical variables like 'Total_Stops', 'Airline', 'Source', and 'Destination' are encoded using one-hot encoding to convert them into numerical form suitable for machine learning algorithms.
The 'Additional_Info' column, which contains non-essential information, is dropped from the dataset.
Feature Visualization:

Data visualization using seaborn and matplotlib is performed to gain insights into the relationships between features and the target variable 'Price'.
Bar plots and box plots are used to visualize the distribution of ticket prices across different airlines.
Model Building and Evaluation:

The dataset is split into training and testing sets using the 'train_test_split' function from sklearn.
A Random Forest Regressor model is created and trained on the training data.
The model's performance is evaluated using various metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Explained Variance Score.
The accuracy of the model is calculated as well.
