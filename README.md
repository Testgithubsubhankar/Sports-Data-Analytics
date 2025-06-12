# Sports-Data-Analytics
Power BI Project
### Dashboard Link : https://app.fabric.microsoft.com/groups/me/reports/73d150bb-9217-4154-b1db-e0d1784a4c8a/ReportSection83b3702888f6d6341c83?redirectedFromSignup=1&experience=power-bi
## Problem Statement
Analysis of India and South Africa matches data Last 20 Years
Data Source-https://stats.espncricinfo.com/

### Steps followed 
1) Web Scraped match statistics using Power BI Web Connector. Also used Invoke function, Query table and Append Function to model the data.
2) Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options
3) Performed data cleaning & transformation using Power Query Editor
4) Modeled data relationships for better insights
5) Designed a dashboard with visuals on team performance, run comparison, player stats & more


Dax Used:

Category = LOOKUPVALUE('Strike Rate Table'[Category],'Strike Rate Table'[Strike Rate],Batting[SR])
Deviation = Abs(Batting[Runs]- AVERAGE(Batting[Runs]))
Rank = RANKX(ALL(Batting),Batting[SR],,DESC,Dense)
Squared Deviation = POWER(Batting[Deviation],2)

Snap of Dashboard:

Batting:
![image](https://github.com/user-attachments/assets/4cf44698-8a2d-453f-8e9d-81c33f16f462)

Bowling:
![image](https://github.com/user-attachments/assets/ed6c52ab-f78b-40f7-99ae-8b93a47c118e)

Fielding:
![image](https://github.com/user-attachments/assets/f243f380-b555-46f3-8f78-baab0041b8f3)


Insight:
Strengthen middle-order batting with consistent No. 4/5 performers.

Enhance fielding drills, especially slip catching and ground fielding.

Prioritize pace-friendly bowling lineups for SA conditions.

Tactical focus on powerplay and death overs.

