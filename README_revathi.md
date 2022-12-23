# Fostering Educational Equity from the Bay to LA
## Author: Revathi Satkuna

## Problem Statement
A board member of an educational policy team for the state of California has entrusted the nonprofit you work at with a grant of $50,000 to distribute within in the Bay Area or Los Angeles in some way, how so is up to you.  They wish for you to identify the best use of the grant so that it could help foster equity within the developing educational world.

## Datasets
### Provided Data
* [`act_2019_ca.csv`](./data/act_2019_ca.csv): 2019 ACT Scores in California by School ([source](https://www.cde.ca.gov/ds/sp/ai/) | [data dictionary](https://www.cde.ca.gov/ds/sp/ai/reclayoutact19.asp))
* [`sat_2019_ca.csv`](./data/sat_2019_ca.csv): 2019 SAT Scores in California by School ([source](https://www.cde.ca.gov/ds/sp/ai/) | [data dictionary](https://www.cde.ca.gov/ds/sp/ai/reclayoutsat19.asp))
### Additional Data
* [`equitabledistric2022.csv`](./data/equitabledistrict2022csv): California Dept of Education Data Public Schools and Districts Data files ([source](https://www.cde.ca.gov/ds/si/ds/pubschls.asp) | [data dictionary](https://www.cde.ca.gov/ds/si/ds/pubschls.asp))

## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|school|object|SAT 2019 Cali|The name of the school|
|district|object|SAT 2019 Cali|The names of the districts in California|
|county|object|SAT 2019 Cali|The counties in California|
|enroll_sr|int64|SAT 2019 Cali|Number of seniors enrolled at the respective high school|
|num_sr_tstaker|int64|SAT 2019 Cali|Number of seniors who had taken the 2019 SAT at that high school|
|participation_rate|float64|ACT 2019 Cali|Number of seniors who had taken the 2019 SAT at that high school divided by the total senior class|
|num_sr_erw_bnchmrk|int64|SAT 2019 Cali|Number of seniors that meet or exceed the benchmark in English, Reading and Writing, meaning they have a 75% chance of earning a C in a first semester college English, Reading and Writing course|
|pct_sr_erw_bnchmrk|float64|SAT 2019 Cali|Percentage of seniors that meet or exceed the benchmark in English, Reading and Writing, that is the number of seniors that have achieved the benchmark divided by total number of seniors at their respective high schools|
|num_sr_mth_bnchmrk|int64|SAT 2019 Cali|Number of seniors that meet or exceed the benchmark in Math, meaning they have a 75% chance of earning a C in a first semester college Math course|
|pct_sr_mth_bnchmrk|float64|SAT 2019 Cali|Percentage of seniors that meet or exceed the benchmark in Math, that is the number of seniors that have achieved the benchmark divided by total number of seniors at their respective high schools|
|tot_sr_bth_bnchmrk|int64|SAT 2019 Cali|Number of seniors that meet or exceed the benchmark in both Math and English, Reading and Writing, meaning they have a 75% chance of earning a C in a first semester college Math or English,Reading and Writing course|
|pct_sr_bth_bnchmrk|float64|SAT 2019 Cali|Percentage of seniors that meet or exceed the benchmark in Math and English, Reading and Writing, that is the number of seniors that have achieved the benchmark divided by total number of seniors at their respective high schools|
|year|int64|SAT 2019 Cali|The year 2019|
|ranking|float64|Expenditure and Income by District|The school districts of California ranked by expenditure of the county per student and average family income of the student's family.|
|score|float64|Expenditure and Income by District|The year 2019|
|expenditure_per_student|float64|Expenditure and Income by District|The average amount of funds the local and federal government will spend on a student's education in a district|
|income_by_district|float64|Expenditure and Income by District|The average household income of a student's family per school district|
|school|object|ACT 2019 Cali|The name of the school|
|district|object|ACT 2019 Cali|The names of the districts in California|
|county|object|ACT 2019 Cali|The counties in California|
|enroll_sr|int64|ACT 2019 Cali|Number of seniors enrolled at the respective high school|
|num_tstaker|int64|ACT 2019 Cali|Number of seniors who had taken the 2019 ACT at that high school|
|num_tstaker|float64|ACT 2019 Cali|Number of seniors who had taken the 2019 ACT at that high school divided by the total senior class|
|participation_rate|float64|SAT 2019 Cali|Number of seniors who had taken the 2019 SAT at that high school divided by the total senior class|
|avg_read_score|int64|ACT 2019 Cali|Average score on the Reading section of the 2019 ACT for the seniors at that high school|
|avg_eng_score|int64|ACT 2019 Cali|Average score on the English section of the 2019 ACT for the seniors at that high school|
|avg_mth_score|int64|ACT 2019 Cali|Average score on the Math section of the 2019 ACT for the seniors at that high school|
|avg_sci_score|int64|ACT 2019 Cali|Average score on the Science section of the 2019 ACT for the seniors at that high school|
|composite_score|int64|ACT 2019 Cali|Sum of the English,Reading, Math and Science section of the 2019 ACT for the seniors at that high school|
|num_ge21|int64|ACT 2019 Cali|The number of seniors at that high school who scored greater than or equal to 21 on the 2019 ACT|
|pct_ge21|float64|ACT 2019 Cali|The percentage of seniors at that high school who scored greater than or equal to 21 on the 2019 ACT|
|year|int64|ACT 2019 Cali|The year 2019|
|ranking|float64|Expenditure and Income by District|The school districts of California ranked by expenditure of the county per student and average family income of the student's family.|
|score|float64|Expenditure and Income by District|The year 2019|
|expenditure_per_student|float64|Expenditure and Income by District|The average amount of funds the local and federal government will spend on a student's education in a district|
|income_by_district|float64|Expenditure and Income by District|The average household income of a student's family per school district|

## Brief Summary of Analysis
- Within the Bay Area, Alameda, Contra Costa and Solano counties tend to be the areas with the lowest incomes.  This corresponds with lower scores.
- In LA, it is Riverside and Ventura counties.
- Composite score on the ACT seems to be positively correlated with participation rate within the Bay and LA. 
- Benchmark score on the SAT and Composite Score in ACT in both English and Math seem to be positively correlated with income.

## Recommendations
- If I were to go with the Bay Area, I would choose Solano, Contra Costa or Alameda counties to use the grant money towards.
- For LA, I would choose either Riverside or Ventura counties. 
- Since household income could be a large contributing factor greatest disparity between scores, facilitating peer-to-peer mentorship programs, providing free to low-cost sliding scale college entrance exam prep can help students from underserved communities get the equity they need to succeed. 


