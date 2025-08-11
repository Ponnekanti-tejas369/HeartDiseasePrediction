# Heart Disease Prediction Using Machine Learning

## Project Overview
This repository contains a machine learning project aimed at predicting heart disease in patients using various health-related features. The dataset used is the Heart Disease dataset, and multiple machine learning models are implemented to classify whether a patient has heart disease.

## Table of Contents
- [Project Overview](#project-overview)
- [Steps Involved](#steps-involved)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Key Observations](#key-observations)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Steps Involved
1. **Data Gathering**: Load the dataset (`HeartDisease.csv`) using pandas.
2. **Data Preparation**: Perform exploratory data analysis (EDA) using pandas functions like `head()`, `tail()`, `describe()`, and `info()` to understand the dataset.
3. **Data Exploration**: Visualize data with histograms, bar plots, correlation matrices, and pair plots to identify relationships between features and the target variable.
4. **Data Preprocessing**: Check for null values and outliers, and convert categorical variables to numerical using one-hot encoding (`pd.get_dummies()`).
5. **Data Transformation**: Standardize numerical features using `StandardScaler` to ensure uniform scaling.
6. **Model Building**: Split the dataset into training (80%) and testing (20%) sets. Train and evaluate the following models:
   - Logistic Regression
   - Support Vector Machine (SVM)
   - Naive Bayes (GaussianNB)
   - Decision Tree Classifier
7. **Model Evaluation**: Assess model performance using accuracy scores, classification reports, and confusion matrices.
8. **Prediction**: Use the trained Support Vector Classifier to predict heart disease for sample inputs.

## Dataset
The dataset (`HeartDisease.csv`) includes the following features:
- `age`: Patient's age
- `gender`: Patient's gender
- `chest_pain`: Type of chest pain
- `rest_bps`: Resting blood pressure
- `cholestrol`: Cholesterol level
- `fasting_blood_sugar`: Fasting blood sugar level
- `rest_ecg`: Resting electrocardiographic results
- `thalach`: Maximum heart rate achieved
- `exer_angina`: Exercise-induced angina
- `old_peak`: ST depression induced by exercise
- `slope`: Slope of the peak exercise ST segment
- `ca`: Number of major vessels colored by fluoroscopy
- `thalassemia`: Thalassemia type
- `target`: Presence of heart disease (0 = No, 1 = Yes)

## Dependencies
The project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-disease-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd heart-disease-prediction
   ```
3. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

## Usage
1. Ensure the `HeartDisease.csv` dataset is in the project directory.
2. Run the main script:
   ```bash
   python heart_disease_prediction.py
   ```
3. The script will:
   - Load and preprocess the dataset
   - Train and evaluate multiple machine learning models
   - Output performance metrics (accuracy, classification report, confusion matrix)
   - Make predictions on sample data using the Support Vector Classifier

## Key Observations
- Features such as `chest_pain`, `rest_ecg`, `exer_angina`, `slope`, `ca`, and `thalassemia` are significantly correlated with the target variable.
- The Support Vector Classifier achieved the highest accuracy among the tested models, making it the most effective for this task.

## File Structure
```
heart-disease-prediction/
│
├── heart_disease_prediction.py  # Main Python script
├── HeartDisease.csv             # Dataset (not included in repo, must be added)
├── README.md                    # Project documentation
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
