# Introduction
Known as one of the oldest beverages in the world, wine has been present since the beginning of civilization, dating back to around 4000 B.C. The first specific tools for wine production and vineyard locations were found from Armenia and Egypt to Greece, France, and Italy. Since then, wine has become one of the most prominent beverages on the planet, to the point where its composition is scientifically studied to improve its quality.

This study aims to better understand the quality of wine and create a Machine Learning model to predict the wine's quality based on its chemical compositions. The model used was the RandomForestClassifier to determine which quality class the wine belongs to.

It is important to note that, although the dataset was sourced from a public data repository, the data presented inconsistencies such as the presence of outliers in the features and the dependent variable, as well as an imbalance in the number of wine quality ratings. Therefore, data preprocessing methods were required to ensure the best accuracy of the created model. Additionally, due to the nature of the features, data standardization was necessary before model creation. Finally, to ensure the integrity of the project's stages, the CRISP-DM methodology will be used to support the project.

# Tools
## Python

- Data Processing: Pandas e Numpy
- library Machine Learning: Scikit-Learn
- Pre processing tools: SMOTE e StandardScaler
- Graphics: Seaborn e Matplotlib
- ML Model: RanonForestClassifier


## Dataset used
  The dataset was public and it was taken form website UCI Machine Learning Repository:

Cortez,Paulo, Cerdeira,A., Almeida,F., Matos,T., and Reis,J.. (2009). Wine Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.


# Main Features and Target

The first step of our project is to understand what is our goals, problemns and how we can deal with it.

So first of all, this dataset is related about a variants of a Portuguese red wine called 'Vinho Verde', so to understand more about the quality of these the owner of this dataset made available the characteristic of the wine that he studied and the classification based of theses features.

The main features avaible on this dataset are:
* fixed acidity
* volatile acidity
* citric acid
* residual sugar
* chlorides
* free sulfur dioxide
* total sulfur dioxide
* density
* pH
* sulphates
* alcohol

And the target of this dataset is:
* quality (score between 0 and 10)

# Structure

## Structure of CRISP-DM
The structure that we will use is based on CRISP-DM method, so it is basically 6 steps to create a project until the depoyment.

  <div align="center">
  <img src="https://github.com/user-attachments/assets/f5b4f818-83b3-42ab-8193-7c994eff5545" width="500px" />
  </div>



## Structure of our project


*  Business Understanding
  * Goals

*  Data Understanding
  *  Splitting the dataset
  * Understanding the distribution
  * Looking for the Outliers
  * Looking for the correlations

* Data Preparation
  * Removing the features
  * Tratment of Outliers
  * Looking the distribution features again
  * Binarize target

* Modeling
  * Preprocess of data
    * Creating the variable train and test
    * Creating the pipeline for preprocess
    * Searching the best model
  * Creating the Pipeline
  * Cross validation
  * Tuning

* Evaluation
  * Nested Cross Validation
  * Confusion Matrix
  * Curve Roc

* Deploy

* Conclusion

# Results
* Result of Nested Cross Validation
  <div align="center">
  <img src="https://github.com/user-attachments/assets/9937b247-fda3-467c-b07c-4b6026248d07" width="150px" />
  </div>
The Nested Cross Validation show that ou model isn't overfitting or underfitting.

* Curve Roc and AUC Score
<div align="center">
<img src="https://github.com/user-attachments/assets/ecfe4eee-0468-43e6-9d1d-632cba112c7f" width="500px" />
</div>

Our project result a good ROC curve and AUC Score, what means that our models is capable to separete new data nicely.

* Confusion Matrix
<div align="center">
<img src="https://github.com/user-attachments/assets/6e4be555-5baf-4e37-acd3-604fe71ba085" width="500px" />
</div>

The confusion matrix show us figurative how hor models is working with the dataset of test, and we can see that our models is capable to classify new data.
