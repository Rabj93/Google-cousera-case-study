# Google-cousera-case-study
cleaning and analyzing data 

Bellabeat Fitness Data Analysis:
The case study follows the six step data analysis process taught in the Google course: Ask, Prepare, Process, Analyse, Share and Act.

Scenario: Since it was founded in 2013, Bellabeat has grown rapidly and quickly positioned itself as a tech-driven wellness company for women. The company has 5 focus products: bellabeat app, leaf, time, spring and bellabeat membership. Bellabeat is a successful small company, but they have the potential to become a larger player in the global smart device market. Our team have been asked to analyze smart device data to gain insight into how consumers are using their smart devices. The insights we discover will then help guide marketing strategy for the company.

The case study follows the six step data analysis process:

1. Ask 
2. Prepare
3. Process
4. Analyze
5. Share 
6. Act

**Step 1: Ask**

BUSINESS TASK: Analyze Fitbit data to gain insight and help guide marketing strategy for Bellabeat to grow as a global player.

Primary stakeholders: Urška Sršen and Sando Mur, executive team members.

Secondary stakeholders: Bellabeat marketing analytics team


**Step 2:  Prepare Data Source:**

30 participants FitBit Fitness Tracker Data from Mobius: https://www.kaggle.com/arashnic/fitbit. This data set was provided with 18 CSV files. 

ROCCC approach:

* Reliablity - LOW, The data provides 30 Fitbit users who consented to use personal tracker data  for activity, sleep, and weight. 

* Orginial - LOW, 3rd party provider

* Comprehensive - Meduim, minute level output for sleep monotoring, heart rate, and phyiscal activity are monitored. 

* Current - LOW, dataset is outdated ranging from March 2016 - May 2016, users habit maybe different now. 

* Citied - LOW, data comes from a 3rd party provider

 The Data has limitions 

* a larger sample would be recommended given that there are only 33 users, we are still able to use the central limit theorem. +
* The data comes from a third-party source with no way to examine credibility or potential biases.


# 3. Process

Tools:
      Microsoft Excel: data cleaning, sorting, filtering, analysis, &    Visualiation
      SQL: data aggregation, transformation, & analysis
      
* Cleaning: Below is a summarry of techniques I used to clean the data

     removing duplicates
     formating the activity date column to YY/DD/MM format
     created a new column using =IF(ISTEXT(cell), value_to_return, "")to 
     days of the week. 
     conditional formating for missing data
     
    
     
 1. First we observe and familiarze ourselve with the data 
 
 ![image.png](attachment:2d69b575-dd1c-4988-b97e-a8117adb9b16.png)
 
 2. Consistency: To start, I identified the standard character length for each user ID (10). Across all tables, there were no    deviations from this and/or incorrect inputs.
 
 3. Check for missing values with COUNTIF( range, criteria ).
 
 4. Remove duplicates with the remove duplicate function in excel. (there are 33 uniques IDS, instead of 30. some users created additional ids during the study period.) 
  
 5. created new column for total minute; with the sum of very, fairly, lightly, and sedentary minutes.
 ![image.png](attachment:42d80852-182d-438a-a533-e6addc9f161a.png)
  
 6. convert Activitydate column from  to mm/yy/dd to yy/mm/dd.
  
  ![image.png](attachment:966f22ce-d0a7-4333-b85a-67df1b7d1f88.png)`
