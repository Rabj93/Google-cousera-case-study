# A Google Data Analytics capstone project. Done in Microsoft Excel and my SQL workbench 

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
 (see issues for pivot tables and graphs) 
 
 2. Consistency: To start, I identified the standard character length for each user ID (10). Across all tables, there were no    deviations from this and/or incorrect inputs.
 
 3. Check for missing values with COUNTIF( range, criteria ).
 
 4. Remove duplicates with the remove duplicate function in excel. (there are 33 uniques IDS, instead of 30. some users created additional ids during the study period.) 
  
 5. created new column for total minute; with the sum of very, fairly, lightly, and sedentary minutes.
  
 6. convert Activitydate column from  to mm/yy/dd to yy/mm/dd.
  
 # 4. Analyze 

performed averages, min, & max using pivot tables

(see issues for pivot tables and graphs) 

# 5.Share

Tracking usage across the week, in the above chart we can see the users usage drop significally during the weekends and picks back up on Tuesday.

 Amount of Calories burned for every step. 
  
  with a positive connection, we can see the increase of calories burned with the range of > 0 - 15,000 steps
  
  As seen from the chart above: 
  
1. Sedentary minutes takes up most of the chart. 
2. This graph shows users tracking daily activities(everyday movements) and not what the app was created for. Given that fairly active and very active minutes are considerably low.


# 6.Act
​
Summary:
​
**Day of the week**
​
The most active days of the week are Tuesday & Saturday 
The least active days of the week are Thursday & Sunday 
​
**Sleep**
​
Users tend to get the most sleep on Sunday & Saturday 
Users get the least amount of sleep on Tuesday & Thursday
There is a positive correlation between sleep and highly active minutes 
The more sleep a user get the more highly active minutes the user will partake in the following day 
​
**Recommendations**
​
* To increase usage, send weekly email campaigns about the importance sleep and     physically activity through the mobile app 
* sendy daily notifications about and evening reminders for bedtime tracking 
* If users are reporting low activty send up to 3 reminders 10am, 3pm, and 6pm to   keep users goals on track
* Send users weekly reports
* Create daily, weekly,and monthly challenges 
​
**Marketing Strategy**
​
* Women heath and wellness blogs 
* Fitnesss influencers on social media (Instagram, Tiktok, etc) 
* Ads and sponsorships
