# <p align = 'center'>Analysis of Motor Collision in New York City (2012 - 2022)</p>

## OVERVIEW:
Within the five boroughs that make up New York City, around 8.2 million people dwell. Thousands of accidents occur each year as a result of a variety of circumstances. The NYPD gathers data on each of these accidents and makes it available to the public on <a href = "nycopendata.socrata.com">nycopendata.socrata.com</a>. We decided to dig deeper into the crash data to see if there were any underlying patterns or relationships that could explain the high frequency of collisions. From `July 2012` to `March 2022`, the data included almost `2,00,000` observations.

## BRIEF - 
* We accessed the data from "nycopendata.com" using `Open Data API` (OData API) and performed Data Connection with Tableau.
* Then, we cleaned the data using Python and stored it in `Google Cloud Storage` as a Bucket to create a virtual instance.
* We performed our analysis using `Google's Big Query` in Google Cloud Platform and stored the query results in CSV files.
* After our analysis, we have generated a report using Google Sites to share our Insights and give Recommendations.

Tableau Story Link: https://public.tableau.com/app/profile/aditya.agarwal1269/viz/NYPDMotorCollisionProject/Story1

Report Link (Google Slides): https://drive.google.com/file/d/16r6KAuHcV5lPYZfqCMQMxOaRkbRwGH77/view?usp=sharing

## DATA DESCRIPTION:
The Motor Vehicle Collisions crash table contains details on the crash event. Each row represents a crash event. The Motor Vehicle Collisions data tables contain information from all police reported motor vehicle collisions in NYC. The police report (MV104-AN) is required to be filled out for collisions where someone is injured or killed, or where there is at least $1000 worth of damage.

Dataset link: https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95

## APPROACH:
1. Understanding the Data - 
It is important to understand our data and our problem statement i.e., how to decrease the number of injuries and deaths in New York City.

2. Preparing the Data -
After understanding our dataset, it is essential to prepare the data. We have used GCP Big Query to remove null values and duplicate entries. 

3. Perform Analysis - 
We have carried out a Time-series analysis and made dashboards to understand more about the factors and causes of Motor collisions in New York City.

4. Get Insights - 
We generated interactive tableau dashboards to support our findings and get insights from the data.

5. Give Recommendations - 
Based on our analysis, we will provide recommendations to decrease the number of Motor collisions.

## QUESTIONS FOR ANALYSIS:
Before exploring the data, we created a list of questions we wanted to address:

1. Is there a trend in the number of accidents?
2. Is there a relationship between the time of day and the contributing factors of the accident? (`Time Series Analysis`)
3. Which areas are more "Collision-prone" areas? (`Collision prone analysis`)

## RESULTS:
1. Analysis performed using `Google Cloud Platform`:

A) Most Injuries and Deaths were caused due to which Vehicle type?

![text](https://github.com/adiag321/NYPD-Motor-Collision-Analysis/blob/ba30e0711a7b01b9d15cf14126d3c17e95719a36/Query_Images/4_Vehicle_Causing_Most_Injuries_Deaths.png)

B) Most of the collisions was caused due to which factor?

![text](https://github.com/adiag321/NYPD-Motor-Collision-Analysis/blob/419b5a57478916001520d70b07c8b3180945a7b5/Query_Images/1_Factor_Highest_Collision.png)

2. Analysis performed using `Tableau`:

A) Detecting Collision-Prone Areas - 

![text](https://github.com/adiag321/NYPD-Motor-Collision-Analysis/blob/419b5a57478916001520d70b07c8b3180945a7b5/Report/Detecting%20Collision%20Prone%20Areas.png)

B) Time Series Analysis - 

![text](https://github.com/adiag321/NYPD-Motor-Collision-Analysis/blob/419b5a57478916001520d70b07c8b3180945a7b5/Report/TIme%20Series%20Analysis%20of%20Motor%20Collision.png)

## INSIGHTS:
1. Between `4 pm to 5 pm` was the peak time of the day when the maximum number of people got injured.
2. The number of people getting injured was `rising from 2012` and was at its peak in `2018` with a value of `123,859 injuries`.
3. In 2018, the total number of injured people decreased to `29,604` injuries in 2022.
4. The highest number of deaths and injuries were majorly caused by a lack of `Driver’s attention.` The other factors also point toward the Driver’s lack of driving skills.
5. Most of the accidents were caused by `Sports utility/Station wagon` vehicles, followed by `Sedan` and `Passenger vehicles`.
6. Also, `4 - wheeled` vehicles were more prone to accidents than `2 - wheeled` vehicles.

## RECOMMENDATIONS:
1. Increase the number of `Traffic Officers` between `4 pm and 6 pm` on days with the highest accident rates.
2. Raise the availability of ambulances between `1 pm to 5 pm` in collision-prone areas.
3. Provide a more robust and efficient `Public transit system` to encourage usage by commuters.
4. Focus on high collision-prone areas such as `11236`, `11207`, and `11234` in prioritizing new projects like traffic lights or street signs.
5. Increase the frequency of `driver re-training` and more `strict fines` for repeat offenders.
6. Increase the `awareness about the use of public transport` the commuters instead of walking or using personal vehicles to reduce accidents.
7. Among all the boroughs, `BROOKLYN` and `QUEENS` had the highest number of deaths in New York City.





