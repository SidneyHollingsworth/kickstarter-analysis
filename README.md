# Analysis of Kickstarter Campaigns

## Overview of Project
Louise recently wrapped up a Kickstarter crowdfunding campaign for her play, ‘Fever’. It, unfortunately, fell just short of the goal. As part of her retrospect, Louise has come to me providing me with an excel file containing historical Kickstarter campaign data to analyze.

### Purpose
The purpose of this analysis is to glean characteristics of Kickstarter campaigns. Louise is particularly interested in how campaigns performed by launch date and funding goals. 

---

### Overview of Analysis: 

To answer Louise's key questions and provide her with actionable insights she can use when designing future Kickstarter campaigns, I used Excel to manipulate, visualize, and analyze provided data.

Prior to performing my analysis, some data cleaning, manipulation, and filtering were needed. For example, provided Unix Timestamp needed to be converted to a more readable and manageable format. Further, 'Category' had to be split into two into 'Parents Category' and 'Sub Category' via split text. The provided dataset included more information than needed. While data on many different types of kickstart campaigns were provided, to perform more relevant analysis for Louise's application, I either filtered to Theater Parent Category or Play Sub Category.  

To explore and analyzed how campaigns performed by launch date and funding goals, I created two pivot charts to create a line chart visualization from each (below).

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
- Percent Successful and Failure almost converged during the month of December.

#### Conclusion: Outcomes based on Goals

-  If I were to recommend a campaign goal range to Louise based on solely campaign outcome and goal, I'd recommend setting a campaign goal of Less than $1,000 to $5,000.
-  Due to the small sample size of campaigns with a goal greater than $15,000, I wouldn't feel comfortable giving a recommendation of confidence.

## Challenges and Limitations

#### Challenges Encountered: 
 
Difficulties encountered when performing my analysis included human error, namely typos in my excel formulas, and having to convert provided Unix Timestamp to a data type more manageable. 

- Human error was overcome by very carefully reviewing all formulas. I had accidentally selected the wrong column when calculating a `=COUNTIF()` formula. It took me about 30min to catch my mistake.
- To convert Unix Timestamp, I used `=(((J2/60)/60)/24)+DATE(1970,1,1)`.

### Dataset limitations
It's important to note that this analysis is quite limited and my conclusions lack confident reliability in application. This project was particularly challenging to me as per the many unknowns and lack of provided context. As a former Marketing Data Analyst, the campaign launch date is of lesser importance than messaging, audience segmentation, and tactics. 

Limitations include but are not limited to:

- The Assumption that the quality and tactics of all campaigns are held equal.
- Small sample size for campaigns with larger goals. For example, there were more campaigns with a goal between $1,000 and $4,999 than total campaigns with goals greater than $4,999.
- The Assumption made about different currencies; unclear as to what kind of impact FX has on the data supplied.
- Campaign Outcome (Successful, Failed, etc.) analyzed in binary terms rather than % Missed relative to Goal. For example, the 'Blood Wedding at Fredriksdal' campaign was short $824 of goal but that's just a 1% difference. 

## Recommended Further Analysis

While one could spend an unlimited amount of time viewing provided data through different filters and views, I'd prioritize the below as part of further analysis creating a 'Missed Percent of Goal' pivot and line chart. After that, it'd be worth filter analysis to country and separately, analyzing standard deviation.
