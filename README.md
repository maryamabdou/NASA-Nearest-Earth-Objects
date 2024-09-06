🚀 Nearest Earth Objects (NEO) Classification Project
NASA Nearest Earth Objects (1910-2024) Dataset
📌 Project Overview
This project involves analyzing and predicting which Nearest Earth Objects (NEOs) pose a potential threat to Earth. Using NASA's dataset, we will clean, preprocess, explore, and model the data to predict whether an object is "hazardous" or "non-hazardous."

Dataset Link: NASA NEO Dataset("https://www.kaggle.com/datasets/ivansher/nasa-nearest-earth-objects-1910-2024/data")

🔧 Project Structure
The following steps were followed in this project:

Data Importing and Cleaning

Imported the dataset using Pandas.
Handled missing values and ensured data integrity.
Dropped irrelevant columns such as object names and other non-informative columns.

Exploratory Data Analysis (EDA)

Performed visual and statistical exploration to understand the distribution of features and the target variable (is_hazardous).
Visualized the distribution of important variables, e.g., absolute_magnitude.

Data Preprocessing

Scaled numerical features to ensure they have similar ranges.
Applied Synthetic Minority Over-sampling Technique (SMOTE) to handle the imbalanced target classes.
Encoded categorical variables using one-hot encoding where necessary.

Model Training and Evaluation

Split the data into training and testing sets.
Trained a Random Forest Classifier to predict whether an object is hazardous.
Evaluated the model using metrics such as Precision, Recall, F1-Score, AUC-ROC, and Balanced Accuracy.

📈 Insights and Findings
Class Imbalance: The dataset is highly imbalanced with very few hazardous objects. SMOTE significantly improved model performance by generating synthetic data for the minority class.
Important Features: Features like absolute_magnitude, est_diameter_min, and est_diameter_max are key predictors of whether an object is hazardous.
Model Performance: The Random Forest Classifier gave excellent results on the balanced dataset, achieving high precision and recall values, along with a high AUC-ROC score.
