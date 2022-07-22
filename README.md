# Final Project

The purpose of this assignment is to analyze salary prediction classification data, and classification on salary whether less than 50K or greater than 50k. The dataset was pulled from Kaggle, the original source is from the US Census database

### Project links
- [Google slide presentation](https://docs.google.com/presentation/d/1e75PlXyeV8oXER-KKV7Z1XRlbs467yrbDvGK3vjCtoo/edit?usp=sharing)
- [Tableau Dashboard](https://public.tableau.com/app/profile/semika.n.burnette/viz/Finalproject_16584483883510/SalaryvsEducation)

## Problem Statement
TBD - Initial ideas - prediction task to determine whether a person makes over 50K a year.  

Our goal is to build a machine learning model that can classify the credit score. 

### Initial ideas for questions we want to answer in predicting a specific target:

- Is there a corelation between education and salaries above or below 50K/yr?
- Prediction of salary based on other demographic indicators. 
- Are there indicators/categories that can accurately predict whether or not an individual will make above 50K/yr?

### Group communication protocols
- Throughout this project the group will communicate through our group slack channel, and WhatsApps as needed.
- This will including sharing information that we find online, code, cleaning up data, aligning on individual tasks, and arranging meetings at least once per week.

### Team Members
- Nelson
- Kelvin
- Semika
- Andrea

### Getting started

We begin the project we searched on Kaggle for possible datasets that would provide us with a robust machine learning dataset to solve for a binary classification problem. 

We located the [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification) dataset that is 3.84 MiB, with 15 columns including information such as age, education, marital status, occupation, race, sex, and other categories that will provide us with meaningful insights for our marchine learning project and analysis. 

### Tools and Resources Used

- [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification) dataset
- GitHub
- Jupyter Notebook

## Segment 2: 

- *Description of preliminary data preprocessing*

In the SQL database, we imported SQLite. We updated the features_df column titles to be more user friendly. SQLite was optimal for our purposes as it connects seamlessly with Jupyter Noteook. We also liked that it has version controls, financial analysis tools, and other features that will make it helpful for our group's online collaboration. Nulls were eliminated when cleaning the data. 

- *Description of preliminary feature engineering and preliminary feature selection, including their decision-making process*

As a group, we spoke about which features we wanted to keep and those that weren't required for our analysis. We decided that the primary key and target columns age and salary. The features/columns that we decided to keep included work_class, education, martital_status, occupation, relationship, race, sex, hours_per_week, and native_country as we believe that we will be able to draw some interesting data and findings with categories based on the target of age and salary. However, we decided to drop some columns that were either ambiguous, or not helpful, for example, 'Education_ID_number" was a column eliminated for our study. 

- *Description of how data was split into training and testing sets*

We created an interjoin between these tables that incorporated the target and the chosen features. We created a connection between sqlite3 and Salary.db, then addded features_df and target_df to our Salary.db. After this, we commited the connection and then executed sql databse in SQLiteStudio. The tables were merged as an OUTERJOIN to complete the full table as this adds the salary column. 

- *Explanation of model choice, including limitations and benefits*

We chose this model for its ability to collaborate seamlessly, track changes, and the features to help with our particular data set for age and salary data targets. Limitations are that some of the data was slow rendering and we needed shut it down and reboot the program a couple times. 

https://public.tableau.com/app/profile/semika.n.burnette/viz/Finalproject_16584483883510/SalaryvsEducation)

The purpose of this assignment is to analyze salary prediction classification data, and classification on salary whether less than 50K or greater than 50k. The dataset was pulled from Kaggle, the original source is from the US Census database.

## Problem Statement
TBD - Initial ideas - prediction task to determine whether a person makes over 50K a year.  

Our goal is to build a machine learning model that can classify the credit score. 

### Initial ideas for questions we want to answer in predicting a specific target:

- Is there a corelation between education and salaries above or below 50K/yr?
- Prediction of salary based on other demographic indicators. 
- Are there indicators/categories that can accurately predict whether or not an individual will make above 50K/yr?

### Group communication protocols
- Throughout this project the group will communicate through our group slack channel, and WhatsApps as needed.
- This will including sharing information that we find online, code, cleaning up data, aligning on individual tasks, and arranging meetings at least once per week.

### Team Members
- Nelson
- Kelvin
- Semika
- Andrea

### Getting started

We begin the project we searched on Kaggle for possible datasets that would provide us with a robust machine learning dataset to solve for a binary classification problem. 

We located the [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification) dataset that is 3.84 MiB, with 15 columns including information such as age, education, marital status, occupation, race, sex, and other categories that will provide us with meaningful insights for our marchine learning project and analysis. 

### Tools and Resources Used

- [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification) dataset
- GitHub
- Jupyter Notebook

## Segment 2: 

- *Description of preliminary data preprocessing*

In the SQL database, we imported SQLite. We updated the features_df column titles to be more user friendly. SQLite was optimal for our purposes as it connects seamlessly with Jupyter Noteook. We also liked that it has version controls, financial analysis tools, and other features that will make it helpful for our group's online collaboration. Nulls were eliminated when cleaning the data. 

- *Description of preliminary feature engineering and preliminary feature selection, including their decision-making process*

As a group, we spoke about which features we wanted to keep and those that weren't required for our analysis. We decided that the primary key and target columns age and salary. The features/columns that we decided to keep included work_class, education, martital_status, occupation, relationship, race, sex, hours_per_week, and native_country as we believe that we will be able to draw some interesting data and findings with categories based on the target of age and salary. However, we decided to drop some columns that were either ambiguous, or not helpful, for example, 'Education_ID_number" was a column eliminated for our study. 

- *Description of how data was split into training and testing sets*

We created an interjoin between these tables that incorporated the target and the chosen features. We created a connection between sqlite3 and Salary.db, then addded features_df and target_df to our Salary.db. After this, we commited the connection and then executed sql databse in SQLiteStudio. The tables were merged as an OUTERJOIN to complete the full table as this adds the salary column. 

- *Explanation of model choice, including limitations and benefits*

We chose this model for its ability to collaborate seamlessly, track changes, and the features to help with our particular data set for age and salary data targets. Limitations are that some of the data was slow rendering and we needed shut it down and reboot the program a couple times. 

## Segment 3:

**Summary**
We conducted 2 different logistical regression: **SMOTE** and **Random Oversampling**. We gaythered data 2 different ways that were both logitical regression.

- Structured outline of the project

We used **Tensorflow** for Random Forest and unsupervised learning.

In this segment we split the data into *testing* and *training*. The X represents the features column, and Y is the target colum. We decided to select salary as the target and dropped the use of age for target. 

When we ran the model our value courts were 24,720 are more or equal to 50k salary per year, and 7,851 are less than 50K per year. 

<img width="485" alt="Segment3modelsalary" src="https://user-images.githubusercontent.com/93094173/180352423-fd29dfe8-bb6e-4375-9790-341898c5dbe8.png">

We used SMOTE Oversampling to oversample which was build off of the test and train split. This method was optimal as a technique to allow us to generate synthetic samples from the minority class and obtain a synthetically class-balanced training set which could be used to train the classifier for our data.









- [Google slide presentation](https://docs.google.com/presentation/d/1e75PlXyeV8oXER-KKV7Z1XRlbs467yrbDvGK3vjCtoo/edit?usp=sharing)
