# Sonar Data Classification with Logistic Regression

## Project Description
This project aims to classify objects detected in sonar signals as either a rock (R) or a mine (M) using a Logistic Regression model. The dataset consists of sonar signals bounced off different surfaces, with each signal represented by 60 numerical features.

## Dataset
The dataset used in this project is `sonar_data.csv`. It contains 208 entries, each with 60 features representing sonar signal patterns and a label indicating whether the object is a 'Rock' (R) or a 'Mine' (M).

## Model
A Logistic Regression model from the `sklearn` library is used for the classification task. The model is trained on a portion of the sonar data and evaluated based on its accuracy on both training and test datasets.

## Dependencies
- `pandas` for data manipulation and analysis.
- `numpy` for numerical operations.
- `sklearn.model_selection.train_test_split` for splitting data into training and testing sets.
- `sklearn.linear_model.LogisticRegression` for the classification model.
- `sklearn.metrics.accuracy_score` for evaluating model performance.

## Usage
1.  **Load Data**: The `sonar_data.csv` file is loaded into a pandas DataFrame.
2.  **Data Preprocessing**: The dataset is separated into features (X) and labels (Y).
3.  **Train-Test Split**: The data is split into training and testing sets (90% training, 10% testing) using `stratify=Y` to maintain class distribution and `random_state=1` for reproducibility.
4.  **Model Training**: A Logistic Regression model is initialized and trained using the training data.
5.  **Model Evaluation**: The model's accuracy is evaluated on both the training and test datasets.
6.  **Prediction System**: A simple predictive system is demonstrated to classify new input data.

### Example Prediction
An example input sonar signal is used to demonstrate how the trained model can predict whether the object is a 'Rock' or a 'Mine'.
