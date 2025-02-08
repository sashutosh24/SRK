Description
This script utilizes supervised machine learning, specifically a Support Vector Machine (SVM) classifier, to predict the success of Bollywood movies based on certain features. It preprocesses the data, trains the model, and evaluates its performance.

Key Functionalities:
Dataset Handling:

Loads a dataset named SRK_12.csv using pandas.
Converts categorical responses like 'Yes' and 'No' into numeric binary values (1 for Yes, 0 for No).
Removes unnecessary columns like 'Movie Title' to focus on predictive features.
Feature and Target Variable Definition:

Defines X (independent features) and y (target variable, Bollywood Blockbuster).
The target column (Bollywood Blockbuster) indicates whether a movie is a blockbuster (1) or not (0).
Data Splitting:

Splits the dataset into training (70%) and testing (30%) sets using train_test_split from sklearn.
Data Preprocessing:

Scales features using StandardScaler for better SVM performance.
Model Training:

Trains a Support Vector Machine (SVM) with a linear kernel using the preprocessed training data.
Model Evaluation:

Evaluates the model using metrics like:
Accuracy Score: Overall correctness of predictions.
Precision: Proportion of true positive predictions.
Recall: Proportion of actual positives identified correctly.
Confusion Matrix: Detailed breakdown of true positives, false positives, true negatives, and false negatives.
Libraries Used:
pandas: For data loading and preprocessing.
sklearn (scikit-learn):
train_test_split: For splitting data into training and testing sets.
SVC: For training the Support Vector Machine classifier.
StandardScaler: For scaling feature values.
metrics: For evaluating the model's performance.
Applications:
Movie Success Prediction: Predict whether a movie will be a blockbuster based on input features.
Feature Analysis: Understand which factors contribute most to movie success.
Decision Support: Aid film producers in understanding potential success based on pre-release attributes.
