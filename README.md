# HeartDiseasePrediction
Heart Disease Prediction Using Machine Learning
Project Overview
This project aims to predict whether a person is suffering from heart disease using machine learning techniques. The dataset used is the Heart Disease dataset, which contains various features related to patient health and a target variable indicating the presence of heart disease.
Steps Involved

Data Gathering: The dataset is loaded using pandas from a CSV file named HeartDisease.csv.
Data Preparation: Initial exploration is performed using pandas functions like head(), tail(), describe(), and info() to understand the dataset's structure and statistics.
Data Exploration: Visualizations such as histograms, bar plots, correlation matrices, and pair plots are used to analyze the relationships between features and the target variable.
Data Preprocessing: The dataset is checked for null values and outliers. Categorical variables are converted to numerical format using one-hot encoding with pd.get_dummies().
Data Transformation: Numerical features are standardized using StandardScaler to ensure all features are on the same scale.
Model Building: The dataset is split into training and testing sets (80/20 split). Four machine learning models are trained and evaluated:
Logistic Regression
Support Vector Machine (SVM)
Naive Bayes (GaussianNB)
Decision Tree Classifier


Model Evaluation: Model performance is assessed using accuracy scores, classification reports, and confusion matrices for both training and testing datasets.
Prediction: The trained Support Vector Classifier is used to make predictions on sample data, determining whether a patient has heart disease.

Key Observations

Features like chest_pain, rest_ecg, exer_angina, slope, ca, and thalassemia show significant correlations with the target variable.
The Support Vector Classifier outperformed other models in terms of accuracy on the test dataset.

Dependencies
The following Python libraries are required to run the code:

pandas
numpy
matplotlib
seaborn
scikit-learn

Install the dependencies using:
pip install pandas numpy matplotlib seaborn scikit-learn

Dataset
The dataset (HeartDisease.csv) contains features such as:

age: Age of the patient
gender: Gender of the patient
chest_pain: Chest pain type
rest_bps: Resting blood pressure
cholestrol: Cholesterol level
fasting_blood_sugar: Fasting blood sugar level
rest_ecg: Resting electrocardiographic results
thalach: Maximum heart rate achieved
exer_angina: Exercise-induced angina
old_peak: ST depression induced by exercise
slope: Slope of the peak exercise ST segment
ca: Number of major vessels colored by fluoroscopy
thalassemia: Thalassemia type
target: Presence of heart disease (0 = No, 1 = Yes)

How to Run

Ensure all dependencies are installed.
Place the HeartDisease.csv dataset in the same directory as the script.
Run the Python script:python heart_disease_prediction.py


The script will output model performance metrics and predictions for sample inputs.

Conclusion
This project demonstrates the application of machine learning to predict heart disease. The Support Vector Classifier achieved the best performance among the tested models, making it a suitable choice for this classification task.
