# Daily Readiness Score Prediction

### Datamining FSS2022 Team6
In this paper, we explored various classification methods to predict one's readiness value for upcoming day. 'Readiness' represents how much some one is ready to do sports.
### Introduction
Life-logging is an activity that helps people to monitor their activity to maintain a healthier lifestyle. Most life log data is stored privately, so individuals cannot easily access to it. As a result of the efforts of Thambawati et al (2020), various analyses of this lifelogging data have become possible. Taking this opportunity, we would like to predict how 'prepared' one would be a day ahead.
### Data
Thambawita et al. provided the dataset explored in this project. Fitbit Versa 2 smartwatch wristband, PMSys sports logging application, and Google form for individual data reporting were used to collect traditional lifelogging data and sports activity logging data. The data was collected over a period of five months (November 2019 to March 2020) and contains information from 16 participants (13 men and 3 women) age between 25 to 60. Participants vary in their background regarding exercise, ranging from someone who rarely exercises to an active athlete.
URL:https://www.kaggle.com/datasets/vlbthambawita/pmdata-a-sports-logging-dataset
![image](https://github.com/kdkangg/Datamining/blob/main/structure.png)
### 
1. agg_Xtrain.csv, agg_ytrain.csv, agg_Xtest.csv, agg_ytest.csv : train,test set aggregated from all participants.

2. agg_Xtest_V2.csv，agg_ytest_V2.csv，agg_Xtrain_V2.csv，agg_ytrain_V2.csv: Erronous pattern in target data has been detected in participant 5's data. Therefore, new train,test set were created.  

3. V2 version of algorithms are corresponding to newly created data in 2.

3. data_aggregation.ipynb is the summary data of all participants

4. data_preprocessing_function.ipynb is used to process each participant's data

7. EDA.ipynb is an Exploratory Data Analysis for datasets

8. Algorithm Plot.ipynb is visualisation of Training Accuracy vs Test Accuracy for different hyperparameters of different methods
