🩺 #Diabetes Data Cleaning Project
This project focuses on cleaning and preparing a dataset related to diabetes diagnosis in Indian patients. The dataset is assumed to come from a CSV file containing medical attributes such as glucose level, insulin, BMI, and more.

📂 Dataset
The dataset is loaded from:

swift
Copy
Edit
C:/Users/NoteBook/Desktop/diabetes.csv
It contains features such as:

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age

Outcome (1: diabetic, 0: non-diabetic)

🧹 Data Cleaning Steps
Handling Missing Values:

Zero values are considered missing in columns like Insulin, BloodPressure, BMI, and SkinThickness.

These zeroes are replaced using appropriate statistics:

Insulin: Replaced by the mean value based on Outcome (separately for diabetic and non-diabetic).

BloodPressure: Replaced by the median.

BMI: Replaced by the mean.

SkinThickness: Replaced by the median.

Data Inspection:

Used .describe() to get summary statistics before and after cleaning.

Used .corr() to examine correlations between variables.

📊 Libraries Used
pandas

numpy
