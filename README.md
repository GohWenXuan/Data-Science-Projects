# GA Project 1: Standardized Test Analysis
## Goh Wen Xuan

## Problem Statement

We are a group of data scientist working for the national College Board who is responsible for developing and administering national-wide SAT/ACT test. In addition, the College Board also provide resources and services to students, colleges and universities in educational planning, adission and financial aid.

The College Board has tasked us to explore if there is a correlation between real GDP per capita and SAT/ACT scores and participation rate, and whether states with higher real GDP per capita produce higher scoring results. This would allow the College Board to determine if additional resources are required to students from lower income states to boost their scores as well as increasing participation rate.

## Executive Summary

This project seeks to study the data for ACT and SAT college exam and their respective participation rates. While only ACT or SAT are mandatory in certain states, having a higher score on ACT/SAT could open up more options for further studies. 

The dataset contains ACT and SAT participation rate, total or composite scores arranged by state level from 2017 to 2019. This allows insights between the participation rates and scores for each state. In addition, a second dataset containing Gross Domestic Product (GDP) of each state is added to explore relationships between a GDP of a state and the ACT/ SAT scores.  

It is observed that there is a negative relationship between participation rate and the ACT and SAT scores. In other words, states with a lowest participation rates are seen to have a higer scores than a state with high participation rate. 

On the other hand, no relationship is found between GDP of a state and the ACT and SAT scores.

## Methodology

The ACT/SAT test scores, participation rates and GDP per capita was imported as PandasDataFrame. All dataframe were analysed for missing values and ensure that all datatypes were accurate and any other errors fixed. Exploratory data analysis was conducted to determine any relationship between the different features. Significant statistical findings were highlighted and visualized using visualization library. The findings were summarised and the recommendations were provided based on the problem statement.

## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|The subnational entities under U.S.A| 
|participation|float|ACT/SAT|The percentage of participants under ACT/ SAT|
|composite|float|ACT|The average of the 4 test scores in ACT|
|ebrw|int|SAT|The score acheived for Evidence-based Reading and Writing for SAT|
|math|int|SAT|The score achieved for Math for SAT|
|total|float|SAT|The sum of the two scores in SAT|
|gdp_per_cap|float|ACT/SAT|The Gross Domestic Product(GDP) per capita of each state|
|act_part_change_17_to_18|float|ACT| The change in percentage for ACT between 2017 and 2018
|act_part_change_18_to_19|float|ACT| The change in percentage for ACT between 2018 and 2019
|sat_part_change_17_to_18|float|SAT| The change in percentage for SAT between 2017 and 2018
|act_part_change_18_to_19|float|SAT| The change in percentage for ACT between 2018 and 2019

## Conclusions and Recommendations

From the state, a moderate correlation is seen between ACT composite score and GDP per capita. In other words, as GDP per capita increases, the average score of ACT increases. However, the same observation could not be seen for SAT.

There is also a distinct negative correlation between participation rates and test scores. As participation rate increases, the lower the ACT/SAT test scores. There is no correlation between GDP per capita and participation rate by state. As a result, it is not necessary to channel additional to poorer states to boost participation. If the College Board aims to solely increase participation rate, it is recommended consider implementing a single, standardised test. This could also be beneficial to both the students and the educational system as it would serve as a benchmark to measure the efficacy of the school. Students could be benefitted in guiding them to appropriate schools.For example, if SAT is mandated in a certain state, the participation rate of ACT is considerably low.

However, keeping in mind that as participation increases, the lower the test score. To aid students in achieving better grades, additional resources could be provided to students from lower-income states, such as subsidies or tuitution grant. Schools could also consider highlighting the importance of the test during school circularium.

## Reference
https://www.princetonreview.com/college/sat-information

https://www.compassprep.com/college-profiles/

https://www.bea.gov/data/gdp/gross-domestic-product 

https://www.mckinsey.com/industries/education/our-insights/the-economic-cost-of-the-us-education-gap  

https://www.jstor.org/stable/1434706
