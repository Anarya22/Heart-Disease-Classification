# Predicting heart disease using machine learning

This notebook looks into various python base ML and DS libraries in an attempt to build a machine-learning model capable of predicting whether or not someone has heart disease based on their medical attributes.

We're going to take the following approach:
1. Problem Definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation

## 1. Problem Definition
In a statement,
> Given clinical parameters about a patient, can we predict whether or not they have heart disease?

## 2. Data
The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease

There is also a version of it available on Kaggle. https://www.kaggle.com/datasets/sumaiyatasmeem/heart-disease-classification-datas

## 3. Evaluation
> If we can reach 95% accuracy in predicting whether or not a patient has heart disease during the proof of concept, we'll pursue the project.

## 4. Features
Which features of the data will be important to us?

Features are different parts and characteristics of the data.
During this step, you'll want to start exploring what each portion of the data relates to and then create a reference you can use to look up later on.
One of the most common ways to do this is to create a data dictionary.
Heart Disease Data Dictionary

A data dictionary describes the data you're dealing with.
The following are the features we'll use to predict our target variable (heart disease or no heart disease).

Feature >  Description >    Example Values
age >	Age in years > 	29, 45, 60
sex >	1 = male; 0 = female >  	0, 1
cp	>    Chest pain type	>   0: Typical angina (chest pain), 1: Atypical angina (chest pain not related to heart), 2: Non-anginal pain (typically esophageal spasms (non heart related), 3: Asymptomatic (chest pain not showing signs of disease)
trestbps >	Resting blood pressure (in mm Hg on admission to the hospital)	>    120, 140, 150
chol >	Serum cholesterol in mg/dl > 	180, 220, 250
fbs >	{Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)}	 >   0, 1
restecg > 	Resting electrocardiographic results > 	0: Nothing to note, 1: ST-T Wave abnormality, 2: Left ventricular hypertrophy
thalach > 	Maximum heart rate achieved > 	160, 180, 190
exang > 	Exercise induced angina (1 = yes; 0 = no) >   	0, 1
oldpeak >	ST depression (heart potentially not getting enough oxygen) induced by exercise relative to rest >	0.5, 1.0, 2.0
slope >	The slope of the peak exercise ST segment >	0: Upsloping, 1: Flatsloping, 2: Downsloping
ca > 	Number of major vessels (0-3) colored by fluoroscopy >	0, 1, 2, 3
thal >	Thalium stress result >	1: Normal, 3: Normal, 6: Fixed defect, 7: Reversible defect
target >   	Have disease or not (1 = yes; 0 = no)	>     0, 1
