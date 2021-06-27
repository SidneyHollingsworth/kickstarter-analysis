# An Analysis of Kickstarter Campaigns

## Overview of Project
Louise recently wrapped up a Kickstarter crowdfunding campaign for her play, ‘Fever’. It unfortunately fell just short of goal. As part of her retrospect, Louise has come to me providing me with an excel file containing historical kickstarter campaign data to analyse.

### Purpose
The purpose of this analysis is to glean characteristics of kickstar campaigns. Louise is particularly interested in how campaigns performed by launch date and funding goals. 

---

### Overview of Analysis: 

To answer Louise's key questions and provide her with actionable insights she can use when designing future kickstarter campaigns, I used Excel to manipulate, visualize, and analyze provided data.

Prior to performing my analysis, some data cleaning, manipulation, and filtering was needed. For example, provided Unix Timestamp needed to be converted to a more readable and manageble format. Further, Category had to be split into two into 'Parents Categorey' and 'Sub Category' via split text. The provided dataset included more information than needed. While data on many different types of kickstart campaigns were provided, to perform more relevant analysis for Louise's application, I either filtered to Theater Parent Category or Play Sub Category.  

To address Louise's key questions, I created two pivot charts to create a line chart visualization from each (below).

### Analysis of Outcomes Based on Launch Date

The below line chart illustrates Outcomes Based on Launch Date.

![image 1](Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

The below line chart illustrates Outcomes Based on Goals.

![image](Resources/Outcomes_vs_Goals.png)

---

## Results

#### Conclusions: Outcomes based on Launch Date

- Theater campaigns launched during the months of May and June performed best while theater campaigns launched during the months of November and December performed worst.
- 

#### Conclusion: Outcomes based on Goals

-  Less Than 1000 and 1000 to 4999 recommended
-  Such a small sample size for campaigns with a goal greater than [X], wouldn't feel comfortable recommending


## Challenges and Limitations

#### Challenges Encountered: 
 
- Difficulties encountered when performing my analysis included human error, namely typos in my excel formulas, and having to convert provided Unix Timestamp to a data type more manageable. Human error was overcome by very carefully reviewing all formulas. To convert Unix Timestamp, I used '=(((J2/60)/60)/24)+DATE(1970,1,1)'.

### Dataset limitations

It's important to note that this analysis is quite limited and my conclusions lack confident reliability in application. This project was particularly challenging to me as per the many unknowns and lack of provided context. As a former Marketing Data Analyst, campaign launch date is of lesser importance than messaging, audience segmentation and tactics. 
- Assumes quality and tactics of all campaigns held equal.
- Small sample size amongst campaigns with larger goal. For example, there were x campaigns with a goal between x and y and z campaigns greater than v.
- Assumption made about different currencies; not sure if goal and outcome data was already converted to dollars
- Outcome of campaigns categorical rather than analysized by difference of pledged from goal

## Recommended Further Analysis

- [possible tables and/or graphs that we could create]
