# Cardiovascular_Risk_Prediction - Classification

**AlmaBetter Verified Project** - [**Credentials**](https://certificates.almabetter.com/en/verify/72713720161696)

![MasterHead](https://d14b9ctw0m6fid.cloudfront.net/ugblog/wp-content/uploads/2021/03/1986.png)

<font size="1">Image Courtesy: https://d14b9ctw0m6fid.cloudfront.net/ugblog/wp-content/uploads/2021/03/1986.png</font>

Click on the following link to checkout the video presentation and the colab file.
- [Colab](https://colab.research.google.com/drive/1tTifv3XpDRYIeVoee8iqIU2ZZe0IWJB1?usp=sharing)
- [Video](https://drive.google.com/file/d/1f9iT1fl29TSW-Uwc0_4cb93LGMUPurDV/view?usp=sharing)


---

## Problem Statement

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients' information. It includes over 4,000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.

---

## Project Summary

The goal of this project was to use machine learning techniques to predict the 10-year risk of future coronary heart disease (CHD) in patients using data from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The dataset provided information on over 4,000 patients and included 15 attributes, each representing a potential risk factor for CHD. These attributes included demographic, behavioral, and medical risk factors.

To prepare the data for analysis, extensive preprocessing was performed to clean and transform the data. This included handling missing values using median, mode, and KNN imputation techniques, as well as identifying and removing outliers using the Interquartile Range (IQR) method. Skewed continuous variables were also transformed using log and square root transformations to reduce skewness and improve model performance.

Feature selection was performed using variance inflation factor to remove multicollinearity and a new feature called pulse pressure was created to capture the relationship between systolic and diastolic blood pressure. Redundant columns were also removed to simplify the dataset. The most important features for predicting CHD risk were identified as ‘age’, ‘sex’, ‘education’, ‘cigs_per_day’, ‘bp_meds’, ‘prevalent_stroke’, ‘prevalent_hyp’, ‘diabetes’, ‘total_cholesterol’, ‘bmi’, ‘heart_rate’, ‘glucose’, and ‘pulse_pressure’.

To handle the imbalanced nature of the dataset, the SMOTE combined with Tomek links undersampling technique was used to balance the class distribution and improve model performance. The data was also scaled using standard scalar method to ensure that all features were on the same scale.

Several machine learning models were evaluated on their performance on the primary evaluation metric of recall. After careful analysis, the Neural Network (tuned) was chosen as the final prediction model because it had the highest recall score among the models evaluated. By selecting a model with a high recall score, the goal was to correctly identify as many patients with CHD risk as possible, even if it meant having some false positives.

Overall, this project demonstrated the potential of machine learning techniques to accurately predict CHD risk in patients using data from a cardiovascular study. By carefully preprocessing and transforming the data, selecting relevant features, and choosing an appropriate model based on its performance on a relevant evaluation metric, it was possible to achieve a positive business impact by accurately predicting CHD risk in patients.

---

## Results

I have selected recall as the primary evaluation metric for our CHD risk prediction model. And after removing the overfitted models which have recall, ROC-AUC, f1 scores for train as 100%, we get the final list:

| Sl. No. | Classification Model      |   Recall Train (%) |   Recall Test (%) |
|:--------|:--------------------------|---------------:|--------------:|
|    1    | Logistic regression       |       72.42  |      73.89 |
|    2    | Logistic regression tuned |       72.42  |      73.89 |
|    3    | Decision Tree tuned       |       80.53 |      68.58 |
|    4    | SVM                       |       72.28 |      72.71 |
|    5    | SVM tuned                 |       91.97 |      74.48 |
|    6    | Naive Bayes               |       65.37 |      74.04 |
|    7    | Naive Bayes tuned         |       66.68 |      69.62 |
|    8    | Neural Network            |       89.45 |      74.04 |
|    9    | Neural Network tuned      |       88.33 |      76.70 |

## Conclusion

In conclusion, this project demonstrated the potential of machine learning techniques to accurately predict the 10-year risk of future coronary heart disease (CHD) in patients using data from an ongoing cardiovascular study. Key points from this project include:

- Careful data preprocessing and transformation improved the performance of machine learning models and enabled more accurate predictions.
- Feature selection was important for identifying the most relevant predictors of CHD risk.
- The Neural Network model (tuned) was chosen as the final prediction model due to its high recall score.
- Techniques such as SMOTE combined with Tomek links undersampling and standard scalar scaling were used to handle imbalanced data and improve model performance.
- This project provides a valuable example of how machine learning techniques can be applied to real-world problems to achieve positive business impact.

Overall, this project highlights the importance of careful data preparation and analysis in machine learning projects. By taking the time to clean and transform the data, select relevant features, and choose an appropriate model, it is possible to achieve accurate predictions and support decision-making in a wide range of domains.

---

## Author

- [Arindam Paul](https://www.linkedin.com/in/arindam-paul-19a085187/)
