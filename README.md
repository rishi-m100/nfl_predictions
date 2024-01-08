# NFL Predictions


## NFL Predictions (WR to receiving yards)
---

Import Libraries: The code starts by importing the necessary libraries - pandas for data manipulation, sklearn for machine learning, and matplotlib for plotting.

Read Data: It reads NFL player data from a CSV file named "yearly_data.csv" into a pandas DataFrame called data.

Select Columns: It then selects specific columns from the DataFrame (selected_columns) related to player performance metrics.

Filter Data for Wide Receivers (WR): It creates a new DataFrame called wr by filtering the original data to include only records where the player's position is 'WR'.

Feature Selection: It further selects features (X) and the target variable (y) for modeling. The selected features exclude 'receiving_yards', 'name', and 'id'.

Train-Test Split: The data is split into training and testing sets using the train_test_split function from sklearn.

Linear Regression Model: It initializes a linear regression model (model) from sklearn, fits it on the training data (X_train, y_train), and prepares to make predictions.

Identify a Player: It sets the variable name to the desired player's name and retrieves their player ID and the most recent season they played.

Retrieve Player Data: It extracts the player's data for the specified season and removes irrelevant columns (desired_player).

Make Prediction: It uses the trained linear regression model to predict the player's receiving yards (y_pred) based on the provided input data (desired_player).

The final result, y_pred, contains the predicted receiving yards for the specified player in the most recent season available in the dataset.