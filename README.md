
# Covid-19 study with AI

  AI offers a way to help us study any kind of data and understand what are the key parameters in a decision. Why not use that to help humanity overcome a disease that led to a pandemic in 2020. We're using AI to **find a better treatment for patients** who might be infected or not.

If you want to learn more about such projects you can checkout my github profile:

https://github.com/OmidAfzali02

  

## Dataset


The dataset was first provided by the Mexican government containing an enormous number of anonymized patient-related information including pre-conditions.

The raw dataset consists of **21 unique features** and 1,048,576 unique patients.

find more information [About Dataset](https://www.kaggle.com/datasets/meirnizri/covid19-dataset) on Kaggle

[Download Dataset](https://www.kaggle.com/datasets/meirnizri/covid19-dataset/download?datasetVersionNumber=1)

# Idea
To understand what parameter effects on the others and how strong or positive or negative the effect is, we can use Ordinary Least Squares Regression or **OLS Regression** to find Correlation.

Correlation is a number which if its positive and a larger number than others we say we have a strong positive correlation between features 1 and 2. Meaning that if feature 1 increases, feature 2 will also increase by a large amount.

The same happens with negative strong correlation to show if feature 1 increases, feature 2 will decrease by a large amount. 
  
  Also weak correlations mean that effect is small whether it's positive or negative.

And at the final after we get a better understanding of important features on our chosen treatment we can use other machine learning algorithms to predict the best treatment for a patient.
Note that OLS Regression offers a model to predict the outcome of the treatment but we  cannot say it's too accurate.

## Important features
As mentioned before we have 21 features on raw dataset. using them all will lead to low accuracy or complication.

As shown on [Data Study.py](https://github.com/OmidAfzali02/Covid-19-study/blob/main/Data%20Study.ipynb) file our features and their Correlation amount with whether the patient has survived or not, is as follows:
|Feature| coef |
|--|--|
| USMER | -0.0048|
| MEDICAL_UNIT| -0.0100|
| SEX| 0.0170|
| PATIENT_TYPE | 0.1073|
| INTUBED| -0.1880|
| PNEUMONIA| -0.0052|
| AGE| 0.0427 |
| PREGNANT| -0.0086 |
| DIABETES| -0.0018|
| COPD| 0.0033|
| ASTHMA| 0.0039|
| INMSUPR| -0.0014|
| HIPERTENSION | -0.0033|
| OTHER_DISEASE| -0.0001|
| CARDIOVASCULAR | 0.0022|
| OBESITY| 0.0022|
| RENAL_CHRONIC| -0.0013|
| TOBACCO| 0.0016 |
| CLASIFFICATION_FINAL| -0.0219|
| ICU| 0.1822|

By this table, we'll sift our features by the largest of positive coef amounts and largest negative coef amounts.

 - strongest positive correlations are: ICU, AGE, PATIENT_TYPE, SEX
 -  Strongest negative correlations are: INTUBED, CLASIFFICATION_FINAL, MEDICAL_UNIT
 - We'll use TOBACCO too just because it's common.

|Feature| coef |
|--|--|
| ICU| 0.1837|
| PATIENT_TYPE| 0.0981|
| AGE| 0.0430|
| SEX| 0.0085|
| TOBACCO| 0.0047|
| INTUBED| -0.1998|
| CLASIFFICATION_FINAL| -0.0221|
| MEDICAL_UNIT| -0.0102|
 

## Predict
In the [Data Study.py](https://github.com/OmidAfzali02/Covid-19-study/blob/main/Data%20Study.ipynb) file you can see a section for prediction. It's used to indicate the death chance of a patient.

The prediction function input form is as follows:

    patient =  [[ICU, PATIENT_TYPE, AGE, SEX, TOBACCO, INTUBED, CLASIFFICATION_FINAL, MEDICAL_UNIT]]

## Recommendation
In the Recommendation section of the code you will enter you patient info like above and after using prediction model on multiple amount of each feature, you'll see what is the best way of taking care of a the patient.

**Note that Recommendation section is not that much reliable and needs the opinion of an expert. If there are any medical experts familiar to this subject, please let me know so we can complete the Recommendation section.**

# How to reach me

.📫 [dev.omid02@gmail.com](mailto:dev.omid02@gmail.com)

. [https://github.com/OmidAfzali02](https://github.com/OmidAfzali02)