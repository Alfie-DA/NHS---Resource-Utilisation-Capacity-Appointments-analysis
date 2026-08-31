
# NHS Appointment Data - Resource-Utilisation-Capacity Analysis
## Project Overview
This project analyses NHS primary care appointment data to identify patterns in appointment demand, capacity utilisation, healthcare professional activity, appointment modes, waiting times and service settings.
The analysis covers appointment activity from August 2021 to June 2022, using Python and data visualisation techniques to transform large-scale healthcare data into actionable operational insights.
The objective was to understand how NHS primary care services were performing over time and identify patterns that could support capacity planning and service improvement.
 
## Business Questions
The analysis investigated six key questions:
1.	How does NHS appointment activity change over time?
2.	How do healthcare professional types differ over time?
3.	Are there significant changes in appointment attendance?
4.	How do appointment modes vary, and which months are busiest?
5.	Are there trends in the time between booking and appointment?
6.	How does appointment activity vary across service settings?
 
## Dataset
The analysis used NHS appointment datasets containing information including:
•	Appointment month
•	Appointment status
•	Healthcare professional type
•	Appointment mode
•	Time between booking and appointment
•	Service setting
•	ICB location
•	Number of appointments
The regional appointment dataset originally covered January 2020 to June 2022. For the main analysis, the data was filtered to August 2021 onwards.
A national categories dataset containing 817,394 records was also used to examine the distribution of appointments across service settings.
 
## Tools & Technologies
•	Python
•	Pandas
•	NumPy
•	Matplotlib
•	Seaborn
•	Jupyter Notebook
 
## Data Preparation
The data preparation process included:
•	Importing CSV and Excel datasets
•	Inspecting data structure and data types
•	Converting appointment month fields to datetime format
•	Filtering the analysis period
•	Grouping appointment records by month
•	Aggregating appointment volumes across healthcare professional types
•	Categorising appointment waiting times
•	Comparing appointment modes and service settings
•	Creating summary measures for daily activity and capacity utilisation
 
## Key Findings
## 1. NHS appointment activity remained consistently high
Across the August 2021–June 2022 period, monthly appointment activity ranged from approximately 23.9 million to 30.4 million appointments.
## The highest monthly volumes were:
### Monthly	Appointments
- November 2021	  -  30,405,070
- October 2021	  -  30,303,834
- March 2022	  -  29,595,038
- September 2021	  -  28,522,501
- May 2022	  -  27,495,508
November 2021 was the busiest month, with more than 30.4 million appointments.
The lowest volume was recorded in August 2021, at approximately 23.9 million appointments.
This represents a difference of approximately 27.5% between the lowest and highest monthly volumes, indicating meaningful variation in demand despite overall consistently high activity.

## Analytical insight
The data does not show a sustained long-term increase or decrease in appointment volumes. Instead, demand fluctuates around a consistently high level, suggesting that NHS primary care services experienced persistent demand rather than a simple upward or downward trend.
 
## 2. Appointment activity showed a clear seasonal pattern
Appointment volumes increased during October and November 2021, reaching their highest levels in November.
Activity subsequently fell during December 2021 and again in April 2022.
The pattern suggests seasonal variation in service activity, potentially associated with:
•	Winter healthcare pressures
•	Christmas holidays
•	Easter holidays
•	Changes in service availability
Importantly, appointment activity recovered after these periods rather than continuing to decline.
## Analytical insight
The rapid recovery following lower-activity periods suggests that the observed reductions were more likely to represent temporary seasonal effects than a sustained reduction in healthcare demand.
 
## 3. Estimated daily activity remained below the 1.2 million/day reference capacity
Monthly appointment volumes were converted into an estimated daily activity measure and compared with a 1.2 million appointments-per-day reference capacity.
Estimated capacity utilisation ranged from approximately:
66.3% to 84.5%
The highest utilisation occurred in November 2021, when estimated daily activity reached approximately:
1,013,502 appointments per day, equivalent to 84.5% of the reference capacity.
The lowest utilisation occurred in August 2021, at approximately:
795,072 appointments per day, equivalent to 66.3% of the reference capacity.

## Analytical insight
The analysis indicates sustained pressure and high activity, but the observed activity did not exceed the reference capacity during the period analysed.
However, appointment volume alone is not sufficient to determine whether NHS staffing levels are adequate. A stronger staffing assessment would require additional information such as workforce levels, available appointment slots, staff workload, patient complexity and local population demand.
 
## 4. General Practitioners consistently accounted for the largest share of appointments
The analysis of healthcare professional types showed that General Practitioners (GPs) consistently delivered the highest volume of appointments throughout the study period.
Other healthcare professionals also made substantial contributions, demonstrating that primary care delivery operates through a multidisciplinary workforce rather than GPs alone.
Seasonal fluctuations were visible across professional groups, particularly around major holiday periods.

## Analytical insight
The findings highlight the central role of GPs while also demonstrating the importance of the wider primary care workforce.
From an operational perspective, capacity planning should therefore consider the contribution of different healthcare professional groups rather than focusing exclusively on GP numbers.
 
## 5. Face-to-face appointments remained the dominant appointment mode
Face-to-face consultations were the most frequently used appointment mode throughout the analysis period.
Telephone appointments consistently represented the second-largest mode and showed relatively stable activity over time.
Home visits and video/online appointments accounted for substantially lower volumes.

## Analytical insight
Despite the availability of remote consultation methods, face-to-face appointments remained the dominant form of primary care access during the period analysed.
The relatively stable level of telephone appointments suggests that remote consultations had become an established component of primary care delivery.
 
## 6. Most appointments were scheduled within relatively short timeframes
Analysis of the time_between_book_and_appointment variable showed that a large proportion of appointments occurred within 0–7 days of booking.
The largest category was same-day appointments, followed by appointments scheduled 2–7 days after booking.
Longer waiting categories were present but represented smaller volumes compared with the shortest waiting periods.

## Analytical insight
The results suggest that primary care services were generally providing appointments within relatively short timeframes during the period analysed.
However, the analysis measures the time between booking and appointment rather than a complete measure of patient waiting time or unmet demand. Further investigation would therefore be required before concluding that access was universally good.
 
## 7. Service-setting activity was highly concentrated in General Practice
The national categories analysis demonstrated substantial variation in appointment volumes across service settings.
General Practice was considerably more prominent than other service settings, highlighting the central role of general practice within the NHS primary care appointment system.
Removing General Practice from the visualisation provided a clearer comparison of the smaller service-setting categories and demonstrated the importance of examining the distribution beyond the dominant category.

## Analytical insight
The strong concentration of activity within General Practice suggests that changes in GP service demand could have a substantial impact on overall primary care activity.
Future analysis should examine whether this concentration varies by geography, population size or demographic characteristics.
 



# Recommendations
## 1. Use seasonal patterns to support capacity planning
The recurring increases in activity during October–November and reductions around December and April suggest that NHS planners could incorporate seasonal patterns into workforce and appointment planning.
Capacity planning should anticipate periods of increased demand rather than relying solely on historical monthly averages.
 
## 2. Investigate regional variation
The analysis identified substantial appointment activity but does not explain why volumes differ between locations.
Further analysis should compare appointment activity against:
•	Local population size
•	Population demographics
•	GP workforce
•	Practice size
•	Rural versus urban location
•	Deprivation levels
This would allow appointment volumes to be interpreted as rates rather than simply absolute counts.
 
## 3. Continue monitoring appointment waiting times
The high proportion of appointments delivered within seven days is encouraging, but waiting-time distributions should be monitored over time.
Future analysis could investigate whether longer waiting categories are concentrated within particular locations, service settings or professional groups.
 
## 4. Evaluate the role of the wider primary care workforce
Because GPs accounted for the largest volume of appointments while other healthcare professionals also contributed substantially, workforce planning should consider the wider multidisciplinary team.
Further analysis could investigate whether some appointment types could be effectively delivered by alternative healthcare professional groups.
 
## 5. Monitor demand against capacity rather than appointment volume alone
The estimated utilisation analysis suggests high activity but does not independently establish staffing adequacy.
A more comprehensive capacity model should combine appointment data with:
•	Workforce data
•	Available appointment slots
•	Staff working hours
•	Patient complexity
•	Population demand
•	Missed appointments
•	Same-day demand
•	Service-level capacity
This would provide a more robust basis for workforce and resource decisions.
 
# Limitations
Several limitations should be considered when interpreting the findings.
Capacity assumption
The analysis compares estimated daily appointment activity against a 1.2 million appointments/day reference figure. This should be treated as a benchmark rather than a definitive measure of operational capacity.
Population differences
Absolute appointment volumes do not account for differences in population size between locations.
Staffing information
The dataset does not contain sufficient workforce information to determine whether staffing levels are appropriate.
Seasonal effects
Changes around Christmas and Easter may reflect changes in service availability as well as changes in patient demand.
Data quality
Records classified as Unknown may reflect missing or incomplete information and should be investigated before making operational decisions.
 
# Business Impact
The analysis demonstrates how healthcare appointment data can support evidence-based decision-making by identifying:
•	Periods of increased demand
•	Seasonal changes in activity
•	Capacity utilisation patterns
•	Workforce contributions
•	Appointment access patterns
•	Differences between appointment modes
•	Variation across service settings
These insights could support healthcare organisations in improving capacity planning, workforce allocation and service monitoring.
 
# Project Structure
nhs-appointments-analysis/
│
├── README.md
│
├── notebooks/
│   └── NHS_Appointment_Analysis.ipynb
│
├── visualisations/
│   ├── monthly_appointment_trends.png
│   ├── capacity_utilisation.png
│   ├── healthcare_professional_trends.png
│   ├── appointment_modes.png
│   └── waiting_time_trends.png
│
└── reports/
    └── analysis_report.pdf
 
# Skills Demonstrated
## Data Analytics
•	Data cleaning
•	Data transformation
•	Exploratory Data Analysis (EDA)
•	Aggregation and grouping
•	Time-series analysis
•	Trend identification
•	Comparative analysis

## Python
•	Pandas
•	NumPy
•	Matplotlib
•	Seaborn
•	Jupyter Notebook

## Data Visualisation
•	Line charts
•	Boxplots
•	Comparative visualisations
•	Trend analysis
•	Capacity analysis

## Business Analysis
•	Translating data into business questions
•	Identifying operational trends
•	Developing evidence-based recommendations
•	Recognising analytical limitations
•	Communicating findings to non-technical stakeholders
 
# Conclusion
The analysis shows that NHS primary care appointment activity remained consistently high between August 2021 and June 2022, with clear seasonal variation and monthly activity ranging from approximately 23.9 million to 30.4 million appointments.
November 2021 represented the peak of activity, while estimated daily utilisation remained between approximately 66% and 85% of the 1.2 million/day reference capacity.
GPs remained the largest contributor to appointment activity, while the wider multidisciplinary workforce played an important supporting role. Face-to-face consultations remained the dominant appointment mode, while most appointments were scheduled within seven days of booking.
Overall, the analysis demonstrates how large-scale healthcare data can be transformed into operational insights while recognising the limitations of using appointment data alone to make decisions about staffing, capacity and patient access.

