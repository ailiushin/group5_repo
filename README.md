***  

# Project 1 - Chicago Crimes 2019-2021
## Team Name: Chi_BearsPy
<br>

### Project Description 
<br>

As a group, we chose to analyze the crime in Chicago. We thought it would be an interesting subject since our group members all live in or around the Chicago area. The subject of crime in Chicago has a long history and we wanted to check on the current trends of crime in our city. We were curious where does most of the crime occur, what time in the day are crimes committed and what crimes are most commonly committed. Through analysis of the crime data we also grew curious of the crimes committed how many of them resulted in arrest. We will use the skills learned in class to present an informational depiction of crime in Chicago.

## Contributors 

Ryan Callaghan, Artem Iliushin, Bhumi Bhusal, Rafael Tem Pahs
<br>   

## Data Source

Data was pulled from: https://data.cityofchicago.org/Public-Safety <br>
CVS files can be found in input folder in the repo: https://github.com/ailiushin/group5_repo.git
<br>

## Technologies
Python, Matplotlib, GoogleMaps
<br>

## Section I <br>
Objective: In this section we analyzed the types of crimes committed. We analyzed which crimes were most commonly committed and which crimes were least commonly committed. We analyzed what the trend of overall crimes committed was from 2019 to 2021.<br>

Approach: We utilized the groupby function and count function. We found that Theft was the most commonly committed crime in total for past three years and Ritualism was the least commonly committed crime. <br>

![Ten Most Common Crimes](https://user-images.githubusercontent.com/99552456/164772226-d6a407bb-df26-4e1f-a47d-bd9396ecdaa4.png)

We also noticed that crime decreased year over year from 2019 to 2021. Which was surprising because we assumed it would increase due to the pandemic and amount of news coverage we noticed.<br>

![Yearly Crime Trend (2019-2021)](https://user-images.githubusercontent.com/99552456/164788861-e1974451-ba93-498b-9862-a208fd864407.png)

## Section II<br>
Objectives: In this section, we wanted to analyze the total number of crimes and total number of arrests in chicago for each of last three years. We also wanted to know percentage of crimes that resulted into arrest for each year. We also wanted to see distribution of crimes by domestic and non-domestic. 
<br>
Approach: We used Pandas dataframe module to separate the data for each year and those with or without arrest. We used bar plots to show trend of crimes and arrests. We also performed statistical analysis using chi-square test, to see if the changes in total number of crimes/arrests are statistically significant. 
<br>
Findings: We found that both number of crimes and arrests reduced for last three years, though the reduction in arrests was more substantial. The changes in both number of crimes and number of arrests were found statistically significant within 95% confidence interval. In addition, we observed that on average, only about 20% of crimes ended up with arrests. It was interesting to observe that, the percentage arrest went down considerably from 2020 to 2021 eventhough, the total number of crimes did not go down at same level. 

![chicago_crime_arrest](https://user-images.githubusercontent.com/99154332/164585329-6f6c5c89-1d8b-48d7-abe8-50b3e7a03796.png)

![Percentage_arrests](https://user-images.githubusercontent.com/99154332/164585436-9080a810-81df-46d8-9aeb-6d20eeb75a70.png)

We also wanted to classify the data into domestic vs non-domestic to see contribution of domestic crimes, and we found that about 20% of crimes were domestic in aggregate.<br>
![Pie_Domestic_vs_nonDomestic](https://user-images.githubusercontent.com/99154332/164585827-b137f3b4-64ba-42b8-861c-92968fa5488f.png)
<br>

## Section III<br>
Objective: In this section we analyzed what is the least dangerous and the most dangerous hour in Chicago based on the three-year period. Further, we wanted to have a visual representation of homicide and concealed carry violations near Loop & Millenium Park area. <br>
Our approach: we utilized a series of code lines to cleanse, aggregate and transform the data to plot the below bar chart. We were extremely surprised to find out that the most dangerous hour in Chicago is 12pm and the safest hour is 5am. Based on our analysis we found that the least number of crimes happen between 1am and 10am. This finding was extremely interesting as our team assumed prior to analyzing the data that most crimes happen after midnight in Chicago.<br> 
![Crimes per Time of the Day (3 years)](https://user-images.githubusercontent.com/100001858/164580296-dc284f7e-82a1-46d3-ac40-b8f581671c78.png)<br>
Further, we utilized google maps api to plot homicide crimes and concealed carry violations. We picked these two types of crimes to visually understand how many severe vs light crimes happened in the loop/millennium park area over the last three years. Based on our analysis we concluded that loop area and millennium park are relatively safe with very little crime occurrence. We think this is mainly due to a large police presence in the area. Two maps below summarize our findings. 
![CONCEALED CARRY LICENSE VIOLATION (3 years)](https://user-images.githubusercontent.com/100001858/164580643-1e5cbb88-5ebd-4a51-a8f2-4f0a30052c03.png) ![HOMICIDES (3 years)](https://user-images.githubusercontent.com/100001858/164580675-ff599e26-6dd0-419d-98a7-46a03169e01f.png)
<br>

## Section IV <br>
We looked at the overall trend of total crimes per district. We further analyzed the total number of crimes per district from 2019 to 2021.The rough map of Chicago below makes it possible to visualize how Chicago is divided. The district with more crimes reported during this period was Jefferson Park, in the North Side of Chicago. Comparing the number of crimes in 2019 with 2021 in Jefferson Park district, the crimes decreased 39.9%
<br>
![mapOfChicago](https://user-images.githubusercontent.com/100001858/164586783-9b5b628b-4605-4106-a13a-334b9b2cd945.jpg)
<br>
![Crimes_per_District](https://user-images.githubusercontent.com/100001858/164586912-6fa10105-ab05-483e-8c5b-99eaec1b95da.png)

## Conclusion
In conclusion, we found out some interesting information about crime in the city of Chicago.  We learned that often crimes committed and reported to police don't lead to arrest. The district with the highest crime totals for the past three years was Jefferson Park. Crime is often committed during the day and not only during the cover of night. Theft and Battery are the most frequently committed types of crime. Finally, crime actually decreased each year from 2019 to 2021, so the state of crime in Chicago has improved over the past two years.
