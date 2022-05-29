# Daily Readiness score prediction with Health data 

### Datamining FS2022 Team6
As interest in healthy lifestyles has increased, gadgets and apps for storing health have become more popular. Wearing a smartwatch or fitness tracker to digitally record your life is a common way to do this. Life-logging is an activity that helps people monitor their activity to maintain a healthier lifestyle. Most life log data is stored privately, so individuals cannot easily access it. As a result of the efforts of Thambawati et al (2020), various analyses of this data have become possible.
Taking this opportunity, we would like to predict how 'prepared' people will be for the day ahead. A person's readiness to exercise can be influenced by the actions and conditions of the previous day. Based on data from the previous day, this project aimed to predict a person's readiness. As the target attribute 'readiness' was stored on a discrete range from 0 to 10, where 0 indicates someone is not ready for exercise on the upcoming day and 10 indicates someone is ready to do additional work, we decided to investigate classification methods.
### Introduction
For our project, we chose to use the Python language and compile it on Jupyter Notebook, an open source web application that allows us to create and share code and documentation. It provides an environment in which you can record code, run code, view results, visualise data and see the output when it is available. These features make it a handy tool for performing end-to-end data science workflows, for data cleaning, statistical modelling, building and training machine learning models, visualising data and many other uses. We collected data from 16 participants and obtained over 10 attributes. We discuss the relevance of each attribute as we believe there are many irrelevant attributes in terms of the format or completeness of the data. In some attributes, zero values were replaced with NaN, so there were some invalid values. There were some outliers and imbalances in the training data because some of the data records were too subjective.
### Data
Thambawita et al. provided the dataset explored in this article. Fitbit Versa 2 smartwatch wristband, PMSys sports logging application, and Google form for individual data reporting are used to collect traditional lifelogging data and sports activity logging data. The data were collected over a period of five months (November 2019 to March 2020) and contains information from 16 participants (13 men and 3 women) ranging in age from 25 to 60. Participants vary in their background regarding exercise, ranging from someone who rarely exercises to an active athlete.
![image](https://github.com/kdkangg/Datamining/blob/main/structure.png)
### Methods
1. agg_Xtrain.csv, agg_ytrain.csv, agg_Xtest.csv, agg_ytest.csv are the training and test sets that have been separated

2. agg_Xtest_V2.csv，agg_ytest_V2.csv，agg_Xtrain_V2.csv，agg_ytrain_V2.csv is the training set and test set after throwing away some invalid 0 values and null values

3. data_aggregation.ipynb is the summary data of all participants and data_aggregation_V2.ipynb is the summary data after removing invalid null and zero values

4. data_preprocessing_function.ipynb is used to process participant data that does not meet the data requirements. We remove the data for participants 08 and 14

5. graph.png is a visualisation of all attributes

6. We used KNN, Decision Tree, MLP, Random forest, SVM, naive_bayes_gaussian methods for prediction, and found a large number of 0 values for readiness (y) of participant 05 by confusion_metrix, and generated separate files, eg: KNN.ipynb; after dropping the 0 values, the method file with the suffix V2 was generated, eg: KNN_V2.ipynb；and integrate the visualised analysis results in run.ipynb

7. EDA.ipynb is an Exploratory Data Analysis for datasets

8. Algorithm Plot.ipynb is visualisation of Training Accuracy vs Test Accuracy for different hyperparameters of different methods
