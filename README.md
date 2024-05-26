# Heart Disease Prediction

This project aims to predict heart disease using various machine learning models. The dataset contains several attributes related to patients' health, such as age, sex, cholesterol levels, and more.

## Dataset

The dataset includes the following attributes:
- Age: age of the patient [years]
- Sex: sex of the patient [M: Male, F: Female]
- ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
- RestingBP: resting blood pressure [mm Hg]
- Cholesterol: serum cholesterol [mm/dl]
- FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
- RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality, LVH: showing probable or definite left ventricular hypertrophy]
- MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]
- ExerciseAngina: exercise-induced angina [Y: Yes, N: No]
- Oldpeak: oldpeak = ST [Numeric value measured in depression]
- ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
- HeartDisease: output class [1: heart disease, 0: Normal]

## Preprocessing

- **Label Encoding**: Binary categorical columns (Sex, ExerciseAngina, FastingBS) were encoded using Label Encoding.
- **One-Hot Encoding**: Multi-class categorical columns (ChestPainType, RestingECG, ST_Slope) were encoded using One-Hot Encoding.
- **Scaling**: Numerical columns were scaled using StandardScaler.

## Models

The following models were trained and evaluated:
- **Support Vector Machine (SVM)**
- **Logistic Regression**
- **Random Forest**

## Results

- **Random Forest** achieved the highest accuracy: 0.9000
- **SVM** and **Logistic Regression** showed slightly lower accuracies.
- **Random Forest with PCA**: Reduced computation time but with lower accuracy: 0.6611

## Visualizations

- **Correlation Matrix Heatmap**: Shows the correlation between different features.
- **Feature Importance Plot**: Displays the importance of each feature for the Random Forest model.

## Conclusion

- **Random Forest** is the best performing model without PCA, achieving the highest accuracy.
- **PCA** helps in reducing computation time but at the cost of accuracy.

