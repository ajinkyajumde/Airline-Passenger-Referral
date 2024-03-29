# Airline-Passenger-Referral
![image](https://user-images.githubusercontent.com/102477662/203225354-8607916b-35fe-4ef3-b4ba-74d58ffb6d1a.png)
# Objective
Detail about airline passenger data referral The given data includes airline reviews from 2006 to 2019 for popular airlines around the world with multiple choice and free text questions. Data is scrapped in Spring 2019. The main objective is to predict whether passengers will refer the airline to their friends. We have tested the data and done some Exploratory data analysis to build machine learning models for the prediction of the dependent factor which is the recommendation of airlines by the passenger to his\her friend.
# ExploratoryData Analysis
The Exploratory Data Analysis (EDA) plays a
vital role in the analysis of the data variables
which are important from the aspect of feature
engineering. It will help us to distribute and
relate between dependent and independent
variables. We have gone through an analysis of
every independent as well as the dependent
variable to check which independent factor
affects the dependent factor.
# Feature Engineering
The given information in its crude structure was not straightforwardly utilized as a contribution to the model. A few components designing was completed where barely any elements were changed, few were dropped, and few were added.We have Engineered new features based on the existing features which are date of travel, review text, overall rating etc. We have done imputation of missing values in the target variable, we also did imputation of missing values in the independent variable. We handled categorical variables and date columns. We used NLP for handling the review text feature.
# Train/Test Split
The train/test split was done as 80/20 % of data with a random state of 0. The final dataset was of shape (61183, 17) which was split to (48946, 17) as Train data and (12237,17) as Test data.
# Machine Learning Algorithms
The machine learning models used are as follows:
## Logistic Regression
Logistic regression is a classification technique that predicts the likelihood of a single-valued result (i.e. a dichotomy). A logistic regression yields a logistic curve with values only ranging from 0 to 1. The likelihood that each input belongs to a specific category is modelled using logistic regression. Logistic regression is a fantastic tool to have in your toolbox for classification purposes.
## Decision Tree

A decision tree is a supervised learning technique used to solve categorization problems. Both categorical and continuous input and output variables are supported.
# Random Forest
We create several trees in the Random Forest model rather than a single tree in the CART model. From the subsets of the original dataset, we create trees. These subsets can contain a small number of columns and rows. Each tree assigns a categorization to a new object based on attributes, and we say that the tree "votes" for that class. The classification with the highest votes is chosen by the forest

# Support Vector Machine
SVM(Support Vector Machine) take a direct approach to binary classification by attempting to find a hyperplane in a feature space that "best" separates the two classes. In practise, however, finding a hyperplane that completely separates the classes using only the original features is challenging. SVMs get around this by expanding the idea of separating hyperplanes in two different ways. (1)Expand the feature space to the point where perfect separation of classes is (more) likely, and(2) apply the so-called kernel trick to extend the feature space.


# Conclusion
In cabin service rating people has given highest recommendation to rating to cabin service rating 5 as compare to its counterpart. From this we can conclude that cabin service is doing pretty good.
In food and beverage rating people have given highest negative recommendation to rating 1.0 from this we can conclude that airline service has to improve their food delivery and quality service.
In entertainment also we can see most people has given highest negative recommendation to entertainment rating 1 which shows that airline has to improve their entertainment system as well.
In ground service also we can see most people has given highest negative recommendation to ground service rating 1 which shows that airline has to improve their ground service.
In value for money also we can see most people has given highest negative recommendation to value for money rating 1 which shows that airline has to make their flight service more cost effective.
In model Selection we can see that Random Forest and XGBoost Model is having the same high Model Accuracy with a score 0.957082 but we can also see that recall, precision, f1-score and roc_auc_score of XGBoost model combined is giving higher score than Random Forest from which we have chosen XGBoost Model for further prediction.
