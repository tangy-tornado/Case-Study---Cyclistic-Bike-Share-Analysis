# Case Study - Cyclistic Bike Share Analysis
Google Data Analytics Professional Certificate - Capstone Project
[Dashboard Link](https://public.tableau.com/app/profile/bharanidharan.m.s/viz/GoogleDataAnalyticsCapstoneProject-Cyclistic_17045484917410/FinalDashboard)

**CYCLISTIC**
➔	Cyclistic, a bike-share company in Chicago, launched in 2016.
➔	Has 5824 bicycles (geotracked), 692 stations.
◆	Only 8% of riders use assistive options.
◆	30% commute to work daily.
➔	3 types -
●	Single ride pass
●	Full day pass
●	Member Usership
➔	To Maximize the number of Member Users.
◆	Rather than creating a marketing campaign to attract new customers.
◆	Convert casual riders to members.

GOAL - Design marketing strategies aimed at converting casual riders into Member Users.

Three questions will guide the future marketing program: 
1. How do Member Users and casual riders use Cyclistic bikes differently? 
2. Why would casual riders buy Cyclistic Member Userships? 
3. How can Cyclistic use digital media to influence casual riders to become members? 

I have been assigned to work on - How Member Users and casual riders use Cyclistic bikes differently? (Identifying themes)


To create a report with the following deliverables: 
1. A clear statement of the business task (ASK)
2. A description of all data sources used (PREPARE)
3. Documentation of any cleaning or manipulation of data (PROCESS)
4. A summary of your analysis (ANALYZE)
5. Supporting visualizations and key findings 3 (SHARE) 
6. Your top three recommendations based on your analysis (ACT)


**ASK **

Guiding questions -
● What is the problem you are trying to solve?
-	The core problem is to address how to increase the conversion rate of casual riders into Member Users at Cyclistic. To solve this, we need to delve into the distinct patterns and behaviors exhibited by Member Users and casual riders when using Cyclistic bikes. By identifying these differences, we will be able to develop targeted marketing strategies that resonate with casual riders, ultimately encouraging them to transition into becoming Member Users of the bike-sharing service. 

● How can your insights drive business decisions? 
-	The insights that I gather from analyzing the differences in behavior between Member Users and casual riders can be phenomenal in shaping key business decisions. 
-	Targeted Marketing Strategies
-	Pricing and Promotions
-	Service Improvements
-	Educating Customers
-	User Experience Enhancements
-	Retention Strategies
-	Operational Efficiency
-	Performance Metrics

Key tasks -
1. Identify the business task 
2. Consider key stakeholders - Lily Moreno, Executive Team

Deliverable -
A clear statement of the business task - 

"Investigate and delineate distinctive usage patterns and behavioral variances between Member Users and casual riders of Cyclistic bikes. This analysis aims to provide insights for crafting precise marketing strategies, with the overarching objective of converting casual riders into Member Users."




**PREPARE**

Guiding questions -
● Where is your data located?
-	Data is in AWS Cloud.
● How is the data organized?
-	Data is organized in tables. With 12 common columns for all data which contain details such as Trip ID, start time, end time, etc., in CSV format.
● Are there issues with bias or credibility in this data? Does your data ROCCC?
-	No, there are no issues with bias or credibility of data, as the data is collected and stored on the company’s server. Yes, it is reliable, original, comprehensive, current and cited.
● How are you addressing licensing, privacy, security, and accessibility? 
-	The data is collected and stored within the company which indeed has its license, and the data doesn’t have any personal information of the customers.
● How did you verify the data’s integrity?
-	Since it is collected and stored within the company servers it is not corrupted and it has a consistent number of columns and data types.
● How does it help you answer your question?
-	It has all the relevant data, but it must be cleaned and filtered to get the necessary insights to proceed further. 
● Are there any problems with the data?
-	Yes, it has a few flaws like null values, inconsistent data type (only in certain columns), and a little more information about customers would have helped (age, gender, etc.). Also, if we got to know customer names, it would have been useful in analyzing whether they use our services often or rarely.

Key tasks -
1. Download data and store it appropriately.
2. Identify how it’s organized. 
3. Sort and filter the data. 
4. Determine the credibility of the data. 

Deliverable - A description of all data sources used.

“The data stored in AWS Cloud is from 2013 - 2023(Nov) but since it has mentioned to use a year's data, I am using the recently available data from Dec 2022 - Nov 2023.”
PROCESS

Guiding questions -
● What tools are you choosing and why?
-	I’m using Excel, R, and Tableau. Since I have cleaned some monthly datasets, I decided to continue the initial cleaning in Excel. The datasets are large, I’ll begin the cleaning process separately for months and then combine them into a single dataset in R and proceed to further cleaning and analysis phase.
● Have you ensured your data’s integrity?
-	Yes, the data is organized and consistent for all the chosen months.
● What steps have you taken to ensure that your data is clean?
-	I have removed unnecessary columns, missing value rows, null values, and duplicate values. Changed columns to correct data type and created additional columns which will be useful for my analysis.
● How can you verify that your data is clean and ready to analyze?
-	I can verify that my data is clean and ready to analyze using Excel and R to find and eliminate null values, duplicates, errors, etc.
● Have you documented your cleaning process so you can review and share those results?
-	Yes, I have documented all the steps taken in the cleaning process in Google Docs.

Key tasks -
1. Check the data for errors. 
2. Choose your tools. 
3. Transform the data so you can work with it effectively. 
4. Document the cleaning process. 

Deliverable -
Documentation of any cleaning or manipulation of data.







**ANALYZE**

Guiding questions - 
● How should you organize your data to perform analysis on it?
-	The data is organized in a CSV format but for my analysis I converted it to Excel workbook format.
● Has your data been properly formatted?
-	No, I have assigned the right data types.
● What surprises did you discover in the data?
-	One of the major surprises was that no Member Users used docked bikes.
● What trends or relationships did you find in the data?
➔	Around 64% of rides in the past 12 months were from Member Users.
➔	Member Users use Classic bike > Electric bike whereas Casual Users use Classic bike > Electric bike > Docked bike.
◆	The important observation was that only Casual Users use docked but it accounts for only 1.84% of total rides.
➔	The highest ride count for Member Users was recorded in August, for Casual Users it was in July. The lowest ride count for Member Users was December, for Casual Users it was January.
◆	I guess most of the Member Users are working professionals so there were fewer rides in December due to Holidays whereas Casual Users use bikes in holidays.
➔	The highest ride count for Member Users is Thursday, for Casual Users it is Saturday. The lowest ride count for Member Users is Sunday, for Casual Users it is Monday.
◆	We can see the rise of Casual Users' rides and the fall of Member Users on weekends.
➔	The highest number of rides during the day peaks at 17:00 hrs. and the lowest is 03:00 hrs. The busiest time is in the Late Afternoon.
➔	When it comes to average ride duration Casual Users outperform Member Users.
◆	It is because the ride count for Casual Users is less and the ride duration is more.
➔	As noticed earlier, the average ride duration of Casual Users significantly peaks on weekends whereas for Member Users it starts to rise once the week starts and stays constant throughout the week but falls once the weekend starts.
● How will these insights help answer your business questions?
-	These insights will help me determine how both types of users use bikes differently and what can be done to convert existing Casual Users into Member Users.

Key tasks - 
1. Aggregate your data so it’s useful and accessible. 
2. Organize and format your data. 
3. Perform calculations. 
4. Identify trends and relationships. 
 
Deliverable - “A summary of your analysis.”


















**SHARE**

Guiding questions - 
●	Were you able to answer the question of how Member riders and casual riders use Cyclistic bikes differently?
-	Yes, with the help of data it was easy to analyze and draw conclusions on how Member Riders and casual riders use bikes differently.
●	What story does your data tell?
-	The main story the data tells us is that Member riders use bikes for routine activities like going to work, but Casual riders use bikes during weekends to travel and hang out.
●	How do your findings relate to your original question?
-	With the help of my findings, we can figure out how to convert existing casual riders to Member Users. Creating a weekend annual pass or aiming to convert casual riders who use docked bikes or casual riders who use electric bikes can be offered some offers and attract them by marketing as eco-friendly rides etc.
●	Who is your audience? What is the best way to communicate with them?
-	My Audience is Lily Moreno and the Marketing analytics team and the best way to communicate is through a presentation of visuals and findings.
●	Can data visualization help you share your findings?
-	Yes, of course. It is the main core of the findings.
●	Is your presentation accessible to your audience?
-	Yes, it is.

Key tasks -
1. Determine the best way to share your findings. 
2. Create effective data visualizations. 
3. Present your findings. 
4. Ensure your work is accessible. 

Deliverable - “Supporting visualizations and key findings.”


 						**ACT**

Guiding questions - 
● What is your conclusion based on your analysis?
-	Member Users use bikes consistently throughout the week and their usage decrease significantly during weekends. Casual Users use bikes significantly more during weekends with longer ride duration when compared to weekdays.
● How could your team and business apply your insights?
-	We can apply marketing strategies to convert Casual Users into annual using my insights. By giving annual weekend passes, giving offers on electric bikes membership passes, and targeting docked bike customers.
● What next steps would you or your stakeholders take based on your findings?
-	They can discuss the findings with the marketing team and business team on how to convert these insights into a successful marketing campaign.
● Is there additional data you could use to expand on your findings?
-	Yes, more info about members' gender and a unique ID for all the members could be useful to find patterns on repeated ride areas and timings.

Key tasks - 
1. Create your portfolio. 
2. Add your case study. 
3. Practice presenting your case study to a friend or family member.

Deliverable - “Your top three recommendations based on your analysis.”

