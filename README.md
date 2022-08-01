# Capstone Project: Airplane Crashes Analysis from 1908 to 2009
# Introduction
After learning Data Analysis with PowerBI in the #NG30daysoflearning organised by [TheOyinbooke](https://twitter.com/TheOyinbooke) and his team, we were asked to showcase what we have learnt in the programme by working on a capstone project and my solution to the project is documented in this report.
# Problem Statement
Ever since the invention of the airplane in 1903 by the Wright Brothers, the transportation industry has experienced a great breakthrough in the effective and nimble movement of individuals from one place to another. There has been an increase in the reproduction of this invention which in turn increases the efficiency of the airplanes while commuting people and goods faster and for more productivity. It is very normal that for every invention made there are backsides which in this case are accidents that happen when they are put to use. Airplane crashes, however, have been a menace since 1908 when the first of its kind happened in the United States causing the death of one of the two people onboard while the other was injured. Over the years these crashes increased as people created and use more airplanes. Moreover, more causes arose causing a shift from failures of all kinds to wars- such as WW1 and WW2, weather, attacks and interference, negligence, and so on.

Accidents are horrific as what happens to people in a plane crash sounds a lot worse—and scarier. It is our duty to study these crashes that have occured over time and get insights into its trends and causes as it affects every country with respect to the operators since inception. This report is therefore deemed to get insights into airplane crashes that occurred between 1908 to 2019.
# Data Sourcing
The data is downloaded from the github datasets provided in [here](https://github.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/blob/main/Airline%20Project/Airplane_Crashes_and_Fatalities_Since_1908.csv)
# Data Transformation
I first loaded the data into Power Query on Excel where most of the cleaning took place. The workbook contained 5,268 rows and 13 columns. I removed some columns such as Flight, Registration and cn/in. Also, I duplicated column twice while I extract column after delimeter for Country column and text before delimeter for State. Added a custom column with an If staement M language to determine the Cause of Accident, courtesy of [Abu Nabeelah](https://twitter.com/Misbaudeen_xls). Code can be found here[M language.txt](https://github.com/adetunjisunday/Airplane-Crashes-Analysis-1908-2009-/files/9234980/M.language.txt). I replaced values manually which was really tasking as I haven't mastered the use of M language much. Values such as states in the United States to were changed to United States and so also those that were not inputted well. Time values that were not enterred correctly were also replaced. Data types were also corrected.

I wrote DAX measures such as Survival rate, Fatality rate, Total Fatalitites, Total Survivors and Total aboard.
# Data visualization
![Airplane Crash 6-1](https://user-images.githubusercontent.com/107109434/182184709-aff24f43-c5eb-42c9-85a8-a9a04a318fb6.png)
[Interact with report here](https://app.powerbi.com/view?r=eyJrIjoiN2Q2NDFmMjctM2FjZS00OWFiLThhZGYtMjlmOGRlNmMxMTdhIiwidCI6ImVhMTJjZDQzLTY2NTYtNDFmYi05NmQwLThlMDkyMjg0YjIzOCJ9)
# Findings
##### Total crashes recorded are 5,268 with 144,551 individuals onboard where fatalities is 105,479 and few survivors of 39,072. This shows that over the years, airplane crashes have always been scary with very high fatality rate common to most of them. There are however few times where people who are not on board are victims of these crashes with total of 8440 individuals recorded so far.

![totals](https://user-images.githubusercontent.com/107109434/182189553-92affbdb-c356-4ebf-ba8a-f00443694317.PNG)

##### United States has the highest contribution to crashes with total of 1344 crashes and a total fatality of 15,392. Aeroflot, however recording highest of total crashes does not contribute in the United States but is largely in Russia and USSR.
Why is United State the highest when Aeroflot is not even in the U.S? This is because other operators which records the ten highest and above crashes and fatalities are prdominantly used in the United States such as Military U.S Airforce, American Airlines, Pan American World Airways, Military U.S. Army Airforces, United Airlines and so on while Aeroflot is the one of the largest and oldest commercial airlines mostly used in Russia and former USSR.

![country](https://user-images.githubusercontent.com/107109434/182192732-a320071f-92fb-4483-bf17-0ee3da92056c.PNG)

##### Structural failure has the highest contribution to accident followed by weather
![cause](https://user-images.githubusercontent.com/107109434/182196994-f107ad2f-c386-4b9b-a4bf-6708fb1f2a78.PNG)

##### Top-10 Operators that contribute to airplane crashes more. Aeroflot is the highest because it is oldest and one of the largest and bussiest commuters of civilians in Russia and USSR is likely majorly prone owing to its sheer size. Aeroflot was once the only airline in operation throughout the whole of the Soviet Union and by the mid-Sixties it was already carrying a remarkable 60 million passengers a year. At the height of the 1970 summer holiday season, it was flying 400,000 passengers a day. 

![operators](https://user-images.githubusercontent.com/107109434/182198098-18a0d77b-58cb-4f25-b80b-460dd65426f7.PNG)

##### 1972, 1985 and 1996 record the top  years with fatalities on passengers on board
There was increase in crashes and fatalities since 1908. However, 1972 set the peak in all the years with 104 crashes and 2,397 fatalities on board plus 30 fatalities on ground before it steeped down to 2009. This later downtrend could possible be because there have been emphasis on safety of airplanes first where these causes were considered before they could take-off and improvement of technology
Also, on Tuesday, September 11, 2001, an American Airline Boeing 767 and United Airlines crashed into the North and West tower of the World Trade Centre in New York city due to a terrorist attack with the highest ground fatality of c. 2,875.

![year](https://user-images.githubusercontent.com/107109434/182241943-32b96a50-3002-4c3a-9641-e007fd7dc098.PNG)

##### The role of warefare in airplane crashes have been traced to the Military US Air-Force operators which came after Aeroflot in number of crashes and fatalities.

![fata](https://user-images.githubusercontent.com/107109434/182253344-24e49f50-bc84-41e3-b10b-9285a4692352.PNG)

# Recommendations
- More airplane safety should be put in place to reduce crashes. These include accurate weather predictions, technical issues should be solved and crosschecked to prevent failures, advanced technological aid in ensuring more safety, enough spaces built in runways and so on.
