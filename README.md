# TechTitans- Stroke-Prediction-Modelling

Kaggle Dataset Link: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset/code 

# Problem Specification
Sometimes referred to as a brain attack, a stroke occurs when blood flow to the brain is impeded or when a blood vessel in the brain ruptures. As a result of this, damage or death of certain regions of the brain can take place. Strokes can potentially result in long-lasting brain impairment, sustained disability, or even death.

Strokes are a major health issue worldwide as well as in Trinidad and Tobago. The Centers for Disease Control and Prevention (CDC) has stated that strokes are the 5th leading cause of death in the United States of America. 6.6 million deaths were attributed to strokes in 2020. According to the World Health Organization (WHO), in 2020, strokes accounted for 822 deaths in Trinidad in Tobago, or 9.56% of total deaths for the year. In 2019, strokes were recorded as the third highest leading cause of death in Trinidad and Tobago.

According to the CDC, 80% of strokes are preventable. Being able to anticipate strokes in patients would therefore help treat those who are at risk of suffering them. Early intervention is critical to minimize the potential damage caused by a stroke. Stroke prediction facilitates early intervention by prompting preventive measures.

# Solution Specification
The aim of this project is to develop a predictive model for stroke detection based on a data set of Stroke data from Kaggle. The data set containes 5110 observations with 12 attributes. Three algorithms were selected for the development of a predictive model. These algorithms are:

Logistic Regression
How it works:

Logistic Regression is linear classification algorithm.
it models probability using the logistic function.
it calculates the weighted sum of input features.
it produces probability score between 0 and 1.
Why it was used:

Logistic Regression is simple and interpretable.
It is well-suited for binary classification tasks such as this.
It makes it easy to understand the relationship between features and stroke likelihood.
It performs well with small datasets such as this.
It is suitable for understanding the impact of individual features on stroke risk
Random Forest Classifier
How it works:

Random Forest Classifier is an ensemble learning algorithm.
It constructs multiple decision trees.
It combines predictions through voting or averaging.
It reduces overfitting through randomness.
Why it was used:

Random Forest Classifier handles complex datasets with high dimensionality.
It is able to capture nonlinear relationships and interactions.
It is robust to outliers and noise.
It reduces the risk of overfitting through ensemble learning.
Feedforward Neural Network
How it works:

A Feedforward Neural Network is an artificial neural network type.
It consists of three layers: input, hidden, output.
It adjusts weights using backpropagation
Its forward pass produces predictions.
Why it was used:

It is able to learn intricate patterns in data.
It automatically extracts features from raw data.
It is adaptable to various data types and structures.
It continuously improves with more data.

# Exploratory Data Analysis (EDA)

Only the main EDA is listed in the README.md
All graphs are listed in the notebook: 

![download](https://github.com/SGajadhar/TechTitans-Stroke-Prediction-Modelling/assets/97929776/d4e6a752-a124-42bd-9d9d-d15f6f33061c)

Observations:
age is by far the attribute with the strongest correlation to strokes.
heart_disease and hypertension both have a similar level of correlation to strokes.
ever_married and avg_glucose have some level of correlation to strokes but it is weaker than the previously mentioned attributes.
bmi, smoking_status, Residence_type, gender, and work_type have little to no correlation with strokes.

![download](https://github.com/SGajadhar/TechTitans-Stroke-Prediction-Modelling/assets/97929776/d29f4113-ece0-4baa-ab4b-410676a1f426)

Observations:
age appears to be the feature with the most importance.

# Data Preprocessing 
In order to remedy the imbalance of the data set, oversampling will be utilised.

# Modelling and Model Tuning 

Notebook Link: 

# Conclusion 

Accuracy Score: Random Forest Classifier achieved the highest accuracy score (0.852), followed by Logistic Regression (0.749), and MLPClassifier (0.718).

ROC AUC Score: Logistic Regression achieved the highest ROC AUC score (0.786), indicating its better ability to distinguish between positive and negative classes compared to the other models.

Precision and Recall: Logistic Regression achieved the highest precision (0.15) and recall (0.66), indicating its ability to correctly classify positive instances while minimizing false positives.

F1 Score: Logistic Regression also achieved the highest F1 score (0.24), indicating a better balance between precision and recall compared to the other models.

Based on these metrics, Logistic Regression seems to be the best-suited model for the problem. It demonstrated the highest ROC AUC score and F1 score among the models, indicating better overall performance in terms of classifying positive instances while controlling false positives.


