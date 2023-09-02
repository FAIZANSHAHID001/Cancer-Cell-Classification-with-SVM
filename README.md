# Cancer-Cell-Classification-with-SVM

**Purpose:**
The purpose of this project is to classify cancer cells as benign or malignant based on certain features extracted from cell samples. We will use Support Vector Machines (SVMs), a popular machine learning algorithm, to build a predictive model for this classification task. The project aims to demonstrate the process of data preprocessing, model training, and evaluation using scikit-learn.

**Functionality of the Project:**

**Data Loading and Exploration:**

Import necessary libraries, including pandas for data manipulation, numpy for numerical operations, and matplotlib for data visualization.
Load the dataset 'cell_samples.csv' using pandas.
Display the last few rows of the dataset using df.tail() to understand its structure.
Count the occurrences of each class label in the 'Class' column using df['Class'].value_counts().

**Data Preprocessing:**

Select a subset of the data for both benign (B_df) and malignant (M_df) classes to create a scatter plot.
Convert the 'BareNuc' column to numeric values and handle any conversion errors or missing values.
Drop the 'ID' column from the DataFrame as it is not needed for classification.

**Data Visualization:**

Create a scatter plot to visualize the data points for both benign and malignant classes using the 'Clump' and 'UnifSize' features.

**Data Preparation:**

Convert the DataFrame into NumPy arrays for machine learning compatibility.
Extract the feature matrix (X) and target vector (Y) for the classification task.
Split the data into training and testing sets using the train_test_split function from scikit-learn.

**Support Vector Machine Model:**

Import the SVM module from scikit-learn.
Create an SVM classifier with a linear kernel, automatic gamma selection ('auto'), and a regularization parameter (C) set to 2.
Train the SVM classifier on the training data using classifier.fit().

**Model Evaluation:**

Use the trained classifier to make predictions on the test data using classifier.predict().
Import the classification_report function from scikit-learn.
Generate a classification report, which includes metrics such as precision, recall, F1-score, and support, to evaluate the model's performance on the test data.

**Printing Results:**

Print the classification report to assess the model's accuracy in classifying benign and malignant cancer cells.
