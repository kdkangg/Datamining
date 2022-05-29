# Daily Readiness Score Prediction

### Datamining FS2022 Team6
As interest in healthy lifestyles has increased, gadgets and apps for storing health have become more popular. Wearing a smartwatch or fitness tracker to digitally record your life is a common way to do this. Life-logging is an activity that helps people monitor their activity to maintain a healthier lifestyle. Most life log data is stored privately, so individuals cannot easily access it. As a result of the efforts of Thambawati et al (2020), various analyses of this data have become possible.
Taking this opportunity, we would like to predict how 'prepared' people will be for the day ahead. A person's readiness to exercise can be influenced by the actions and conditions of the previous day. Based on data from the previous day, this project aimed to predict a person's readiness. As the target attribute 'readiness' was stored on a discrete range from 0 to 10, where 0 indicates someone is not ready for exercise on the upcoming day and 10 indicates someone is ready to do additional work, we decided to investigate classification methods.
### Introduction
Life-logging is an activity that helps people monitor their activity to maintain a healthier lifestyle. Most life log data is stored privately, so individuals cannot easily access it. As a result of the efforts of Thambawati et al (2020), various analyses of this data have become possible. Taking this opportunity, we would like to predict how 'prepared' one will be for the day ahead.
### Data
Thambawita et al. provided the dataset explored in this article. Fitbit Versa 2 smartwatch wristband, PMSys sports logging application, and Google form for individual data reporting are used to collect traditional lifelogging data and sports activity logging data. The data were collected over a period of five months (November 2019 to March 2020) and contains information from 16 participants (13 men and 3 women) ranging in age from 25 to 60. Participants vary in their background regarding exercise, ranging from someone who rarely exercises to an active athlete.
URL:https://www.kaggle.com/datasets/vlbthambawita/pmdata-a-sports-logging-dataset
![image](https://github.com/kdkangg/Datamining/blob/main/structure.png)
### Different section
1. agg_Xtrain.csv, agg_ytrain.csv, agg_Xtest.csv, agg_ytest.csv are train,test set aggregated from all participants.

2. cluster readiness 5 is mostly collided with readiness 0, so those are assumed as erroneous. Based on our assumption, algorithms were run again using a dropped zero readiness score on person 5 ,so we create new train,test set as agg_Xtest_V2.csv，agg_ytest_V2.csv，agg_Xtrain_V2.csv，agg_ytrain_V2.csv and we used KNN, Decision Tree, MLP, Random forest, SVM, naive_bayes_gaussian methods for prediction, so we create new file with the suffix V2 was generated eg:  KNN.ipynb vs. KNN_V2.ipynb；and integrate the visualised analysis results in run.ipynb

3. data_aggregation.ipynb is the summary data of all participants

4. data_preprocessing_function.ipynb is used to process participant data that does not meet the data requirements. We remove the data for participants 08 and 14

7. EDA.ipynb is an Exploratory Data Analysis for datasets

8. Algorithm Plot.ipynb is visualisation of Training Accuracy vs Test Accuracy for different hyperparameters of different methods
