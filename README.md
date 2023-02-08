
# Covid-19 study with AI

  AI offers a way to help us study any kind of data and understand what are the key parameters in a decision. Why not use that to help humanity overcome a disease that led to a pandemic in 2020. We're using AI to find a better treatment for patients who might be infected or not.

If you want to learn more about such projects you can checkout my github profile:

https://github.com/OmidAfzali02

  

## Dataset


The dataset was first provided by the Mexican government containing an enormous number of anonymized patient-related information including pre-conditions.

The raw dataset consists of 21 unique features and 1,048,576 unique patients.

find more information [About Dataset](https://www.kaggle.com/datasets/meirnizri/covid19-dataset) on Kaggle

[Download Dataset](https://www.kaggle.com/datasets/meirnizri/covid19-dataset/download?datasetVersionNumber=1)

# Idea
To understand what parameter effects on the others and how strong or positive or negative the effect is, we can use Ordinary Least Squares Regression or OLS Regression to find Correlation.

Correlation is a number which if its positive and a larger number than others we say we have a strong positive correlation between features 1 and 2. Meaning that if feature 1 increases, feature 2 will also increase by a large amount.

The same happens with negative strong correlation to show if feature 1 increases, feature 2 will decrease by a large amount. 
  
  Also weak correlations mean that effect is small whether it's positive or negative.

And at the final after we get a better understanding of important features on our chosen treatment we can use other machine learning algorithms to predict the best treatment for a patient.
Note that OLS Regression offers a model to predict the outcome of the treatment but we  cannot say it's too accurate.

## Important features
As mentioned before we have 21 features on raw dataset. using them all will lead to low accuracy or complication.

As shown on [Data Study.py](https://github.com/OmidAfzali02/Covid-19-study/blob/main/Data%20Study.ipynb) file our features and their Correlation amount with whether the patient has survived or not, is as follows:



# How to reach me

.📫 [dev.omid02@gmail.com](mailto:dev.omid02@gmail.com)

. [https://github.com/OmidAfzali02](https://github.com/OmidAfzali02)