# Heart-Attack-Prediction
1. The aim of this project is to predict the risk of heart attack to a particular individual.
2. The dataset is the past information of the patients about their health statues.
3. This Dataset has 26 features and about 9000 samples. (You can get the dataset from this repository or you can download it from 
4. Age, Sex, Blood Pressure, Alcohol Consumption, Smoking, etc.. are some of the features.


# Model Summary
1. Starting with the Data cleaning, as the dataset doesn't contain any null values,duplicates and outliers.
2. As the column 'Patient_ID' is just an unique identifier of the patient, it does affect on model's perfomance. So, it has dropped.
3. Followed by Data Preprocessing, I observed that target variable is slightly imbalnced, so i have resampled the data using SMOTE.
4. After, I have performed feature engineering techniques like chi_2 test, found mutual info classification values and variance inflation factor (VIF) values to remove irrelevant features.
5. Then Tested with some known algorithms like Logistic Regression, Decision Tree, K-Nearest Neighbors and Random Forest Classifier and hypertuned with GridSearchCV.
6. Observed better accuracy and precision fot Random Forest Classifier than other three.
7. Then implemented a neural network with 3 dense layers(including output layer). Trained the model with different no of neurons to get the optimum accuracy and precison.
8. As this is an Heart Attack Risk Prediction, I have also focussed on precision.

# Conclusion
1. The dataset shouls have more samples about the patients who are suffere with Heart Attack. Because of less information about them, the dataset is slighlty biased, still after re-sampling, it doesn't improved much.
2. When removing the features, I thought many of them will definetely affect the output but unfortunately they were removed due to when performing feature engineering (because of more VIF, high p-value in chi_2 test or very less mutual-information value)
3. Still, upto some level, this model performs well but more information would have made it better.
