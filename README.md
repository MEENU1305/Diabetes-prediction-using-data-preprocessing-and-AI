Data Preparation 


FEATURE ENGINEERING & DATA PRE-PROCESSING

Feature engineering and Data Pre-Processing are the most significant topics in data science. In a general opinion, 80% of the work is data preprocessing, and 20% of the work is modeling in a machine learning project, therefore, there are issues to be considered. The aim of this notebook is to be a tutorial on the approach to data preparation.



Feature Engineering: The work performed on the features (such as preprocessing, generating a new variable, etc.), and generating variables from raw data.

Data Preprocessing: The process of making the data suitable before implementing a model.

In this step, there are 4 topics to consider and handle to prepare the dataset.

Outliers
Missing Values
Feature Extraction
Encoding & Scaling
All of these are the steps of data preprocessing and feature engineering, and each of them will be explained in the notebook.

Obviously, before the process, the dataset has to be explored, and the variables have to be understood. That means the dataset has to be prepared before preparing. Make ready to your popcorns for the movie named "Inception on Data Science"! Of course, it does not that hard, but there are rules and steps to be followed in order to not get lost.



 First look to the Dataset

Business Problem: It is desired to develop a machine learning model that can predict whether people have diabetes when their characteristics are specified. You are expected to perform the necessary data analysis and feature engineering steps before developing the model.

Story of Dataset: 

The dataset is part of the large dataset held at the National Institutes of Diabetes-Digestive-Kidney Diseases in the USA. Data used for diabetes research on Pima Indian women aged 21 and over living in Phoenix, the 5th largest city of the State of Arizona in the USA.

Variables: The target variable is specified as "outcome"; 1 indicates positive diabetes test result, 0 indicates negative.

Pregnancies: The number of pregnancies

Glucose: 2-hour plasma glucose concentration in the oral glucose tolerance test

Blood Pressure: Blood Pressure (Small blood pressure) (mmHg)

SkinThickness: Skin Thickness

Insulin: 2-hour serum insulin (mu U/ml)

DiabetesPedigreeFunction: A function that calculates the probability of having diabetes according to the descendants

BMI: Body mass index

Age: Age (year)

Outcome: Have the disease (1) or not (0)

 EDA (Exploratory Data Analysis)
   
This is the part of the explore the dataset. The outliers and missing value analyses will be done in this part but the only point is to observe these in this part. The operation and editing for these will be done in Part 3: Pre-processing.

2.1 Analyse outliers and missing values¶
 The only process in EDA is to analyze the values. Editing of missing values and outliers will be done in the next part.

Outliers
Values that deviate considerably from the general trend in the data are called outliers. Especially in linear problems, the effects of outliers are more severe. They have less impact on tree methods, but still, need to be considered.

How are outliers determined?:
The critical point is to determine the acceptable threshold value, which are up limit and low limit. After determining the threshold value, outliers are caught based on these values. Methods by which we can catch the threshold value:

Industry knowledge,
Standard deviation approach,
Z-score approximation,
Boxplot(interquartile range-IQR) method (as univariate),
LOF Method => Multivariate.
