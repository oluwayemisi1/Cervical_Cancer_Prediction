# Cervical_Cancer_Prediction
# Introduction
Cervical cancer is a significant health concern globally, particularly in low- and middle-income countries where regular screening and early detection are less accessible. The disease is primarily caused by persistent infection with high-risk human papillomavirus (HPV) types, making it a preventable and treatable condition if detected early. However, many women still face the risk of late-stage diagnosis, leading to higher mortality rates. The integration of machine learning models in the prediction and early diagnosis of cervical cancer can potentially reduce these risks by identifying high-risk individuals based on various factors and enabling timely intervention.

## Contents
1. Aim and objectives
2. Data Sourcing 
3. Data Preprocessing
4. Exporatory Data Analysis
5. Findings
6. Conclusion

## Aim and Objectives

The aim of this project is to develop a predictive model that can accurately assess the risk of cervical cancer in individuals..The use of machine learning algorithms, the project seeks to improve the early detection of cervical cancer, thereby aiding in the prevention and management of this disease.

Objectives
    Data Understanding: I explored and understood the key variables
    Data Preprocessing: I cleaned the dataset and handled missing values,Converted specified columns to binary values..
    Exploratory Data Analysis: I analyzed the data to identify patterns and relationships.
    Feature Engineering: I selected the important features for prediction Model Development: I built machine learning models to predict cervical cancer risk.
    Model Evaluation:I evaluated the model performance using accuracy and other metrics.
    Google Colab Implementation: I implemented the entire process in Google Colab.

# Dataset
This cervical cancer dataset contains medical and demographic information about individuals, focusing on risk factors associated with cervical cancer. It includes features such as age, number of sexual partners, age at first sexual intercourse, pregnancy history, smoking habits, use of hormonal contraceptives and intrauterine devices (IUDs), and history of sexually transmitted diseases (STDs). The dataset includes results from cervical cancer detection tests like Hinselmann, Schiller, cytology, and biopsy. The data was used to build machine learning models aimed at predicting cervical cancer diagnoses, helping in early detection and improving patient outcomes.

# Data Preprocessing
The dataset had inconsistent decimal precision in float columns, non-binary categorical data, and missing values that needed to be addressed for accurate analysis. In this preprocessing step, float columns in the dataset were rounded to two decimal places to ensure consistency. Specific categorical columns related to smoking, contraceptive use, and STDs were then converted into binary format, with values of 0 and 1, based on a threshold of 0.5. Finally, missing values were filled with the column means to maintain data integrity, preparing the dataset for further analysis.

# Exporatory Data Analysis
1. A combination of a scatter plot and line plot was done to know the Relationship between First Sexual Intercourse and Various STD-related Metrics:
The number of diagnoses tends to decrease as the age of first sexual intercourse increases, with some fluctuations. The time since first and last diagnoses remains relatively stable, though there are notable drops at certain ages, indicating potential data variability or outliers.
2. A box plot was carried out to  shows the age distribution across different diagnoses, such as cancer, CIN, HPV, and others. The median age for most diagnoses appears to be in the 30s, with some outliers in older age groups. The spread of ages varies, with some diagnoses showing a wider range, indicating variability in the age at which individuals are diagnosed. The plot suggests that certain conditions might be diagnosed across a broader age range than others.
3. A bar chart was done to compares the distribution of the number of pregnancies between those who have used hormonal contraceptives and those who have not, showing that users of hormonal contraceptives generally have more pregnancies.
4. A bar plot was carried out to know the Distribution of Smoking Years by Smoking Status, and the findigs shows that the individuals who smoke was more than the indivisuals who doesn't smoke.
5. A bar plot was carried out to know the Distribution of Hormonal Contraceptives Years by Hormonal Contraceptives Status, the findings shows that There is a higher number of individuals with many years of contraceptive use compared to those with fewer years of no contraceptive use.
6. A scatter plot was done to know the Age Distribution with people with Cancer Diagnosis, The scatter plot shows that people with cancer were more commonly aged between 20-50, with a sparse distribution across this range, while those without cancer were clustered between 15-45, with fewer cases appearing around age 80.

# Modelling
1. Random Forest (RF): 100%
2. Support Vector Machine (SVM): 98.20%
3. Logistic Regression (LR): Mean Squared Error: 0.0126, R-squared: 0.4583
5. AdaBoost: 98.80%
6. CatBoost: 100%

Among these models, Random Forest achieved the highest accuracy, making it the most effective for predicting cervical cancer risk in this case.

# Findings
One key finding from the analysis is that individuals with an earlier age of first sexual intercourse tend to have a higher likelihood of being diagnosed with sexually transmitted diseases (STDs), highlighting the significance of early sexual health education and intervention in reducing cervical cancer risk. The Random Forest and CatBoost model achieved the highest accuracy of 99.40% in predicting cervical cancer risk, indicating its effectiveness in distinguishing between individuals at high and low risk for the disease.

# CONCLUSION
I conclusion This project successfully demonstrated the importance of machine learning models in predicting cervical cancer risk, with the Random Forest and CatBoost algorithm achieving the highest accuracy of 100%, which shows the model's effectiveness in identifying individuals at risk. By applying machine learning techniques and detailed data analysis, this project contributes to improving cervical cancer screening processes and potentially reducing the incidence and mortality associated with the disease. The application of AI in clinical practice could enhance early detection efforts, leading to earlier diagnoses of cervical cancer and facilitating timely treatment.
