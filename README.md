# heartdiseaseprediction
Importing Dependencies: This section imports necessary libraries for data manipulation, machine learning, and evaluation, including NumPy, pandas, scikit-learn's train_test_split, LogisticRegression, and accuracy_score.

Data Collection and Processing: In this section, the script loads heart disease data from a URL using pandas, replaces missing values with pd.NA, drops rows with missing values, prints the first and last few rows of the dataset, and provides information about the dataset using shape, info, isnull, and describe functions.

Splitting the Features and Target: The dataset is split into features (X) and the target variable (Y) representing whether a person has a heart disease. X contains all columns except the 'target', and Y contains the 'target' column.

Splitting the Data into Training and Test Data: The dataset is further split into training and test sets using the train_test_split function. It splits the data into 80% training and 20% test sets while ensuring that the distribution of the target variable is maintained in both sets.

Model Training: A logistic regression model is created using scikit-learn's LogisticRegression class and trained on the training data using the fit method.

Model Evaluation: The trained model's accuracy is evaluated on both the training and test data using the accuracy_score function. The accuracy on training data and test data is printed.

Building a Predictive System: An example input data point is defined, and its feature values are stored in a dictionary. The input is converted to a numpy array, reshaped, and passed to the trained model for prediction. Depending on the prediction, it prints whether the person has a heart disease or not.

The purpose of this code is to showcase a basic implementation of a logistic regression model for heart disease prediction, including data preprocessing, model training, evaluation, and making predictions on new data points.
