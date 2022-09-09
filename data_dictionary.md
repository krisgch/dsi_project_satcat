# Project 1: Standardized Test Analysis - Data Dictionary

---

## Cleaned Datasets

#### States Data
* [`sat_df_cleaned.csv`](./data/cleaned/sat_df_cleaned.csv): Cleaned and combined 2017-19 SAT Scores by States
* [`act_df_cleaned.csv`](./data/cleaned/act_df_cleaned.csv): Cleaned and combined 2017-19 ACT Scores by States

#### California Data
* [`sat_2019_ca_df_cleaned.csv`](./data/cleaned/sat_2019_ca_df_cleaned.csv): Cleaned california SAT performance by schools in 2019
* [`sat_2019_ca_11_cleaned.csv`](./data/cleaned/sat_2019_ca_11_cleaned.csv): Cleaned california SAT performance by schools in 2019 (grade 11 only)
* [`sat_2019_ca_12_cleaned.csv`](./data/cleaned/sat_2019_ca_11_cleaned.csv): Cleaned california SAT performance by schools in 2019 (grade 12 only)
* [`sat_2019_ca_both_cleaned.csv`](./data/cleaned/sat_2019_ca_both_cleaned.csv): Cleaned california SAT performance by schools in 2019 (both grades)
* [`act_2019_ca_df_cleaned.csv`](./data/cleaned/act_2019_ca_df_cleaned.csv): Cleaned california ACT performance by schools in 2019

#### General College Data
* [`sat_act_by_college_cleaned.csv`](./data/cleaned/sat_act_by_college_cleaned.csv): Cleaned accepted SAT and ACT by each college
* [`sat_2019_by_college_major_cleaned.csv`](./data/cleaned/sat_2019_by_college_major_cleaned.csv): Cleaned score by intended college major

#### Additional Data
* [`ca_capita_wiki.csv`](./data/cleaned/ca_capita_wiki.csv): Cleaned list of California locations by income


## Cleaned Data Dictionary

#### States Data

*sat_df_cleaned*

|Field #|Field Name|Type|Dataset|Description|
|---|---|---|---|---|
|0|state|str|sat_df|State in the US|
|1|participation|float|sat_df|Percentage test takers from this state|
|2|reading_writing|int64|sat_df|Average reading & writing score|
|3|maths|int64|sat_df|Average maths score|
|4|total|int64|sat_df|Average total score|
|5|year|int64|sat_df|Year of test|

*act_df_cleaned*

|Field #|Field Name|Type|Dataset|Description|
|---|---|---|---|---|
|0|state|str|act_df|State in the US|
|1|participation|float|act_df|Percentage test takers from this state|
|2|composite|float|act_df|Average composite score|
|3|year|int64|act_df|Year of test|


#### California Data

*act_2019_ca*

|Field #|Field Name|Type|Dataset|Description|
|---|---|---|---|---|
|1|cds_code|float|act_2019_ca|County/District/School Code|
|2|county_code|float|act_2019_ca|County Code|
|3|district_code|float|act_2019_ca|District Code|
|4|school_code|str|act_2019_ca|School Code|
|5|record_type|str|act_2019_ca|Record Type: C=County, D=District, S=School, X=State|
|6|school_name|str|act_2019_ca|School Name, N/A = County or District Level Record|
|7|district_name|str|act_2019_ca|District/LEA Name, N/A = County Level Record|
|8|county_name|str|act_2019_ca|County Name|
|9|grade_12_enroll|float|act_2019_ca|Enrollment of Grade 12|
|10|test_takers|float|act_2019_ca|Number of Test Takers|
|11|avg_reading_score|str|act_2019_ca|Average ACT Reading Score|
|12|avg_english_score|str|act_2019_ca|Average ACT English Score|
|13|avg_maths_score|str|act_2019_ca|Average ACT Maths Score|
|14|avg_science_score|str|act_2019_ca|Average ACT Science Score|
|15|num_ge_21|str|act_2019_ca|Number of Test Takers Whose ACT Composite Scores Are Greater or Equal to 21.|
|16|pct_ge_21|str|act_2019_ca|Percent of Test Takers Whose ACT Composite Scores Are Greater or Equal to 21.|
|16|year|str|act_2019_ca|The ACT test administration year: 2018-19|

*sat_2019_ca*

|Field #|Field Name|Type|Dataset|Description|
|---|---|---|---|---|
|0|cds_code|float|sat_2019_ca|County/District/School Code|
|1|county_code|float|sat_2019_ca|County Code|
|2|district_code|float|sat_2019_ca|District Code|
|3|school_code|float|sat_2019_ca|School Code|
|4|record_type|str|sat_2019_ca|Record Type: C=County, D=District, S=School, X=State|
|5|school_name|str|sat_2019_ca|School Name, N/A = County or District Level Record|
|6|district_name|str|sat_2019_ca|District/LEA Name, N/A = County Level Record|
|7|county_name|str|sat_2019_ca|County Name|
|8|grade_11_enroll|float|sat_2019_ca|Enrollment of Grade 11|
|9|grade_11_takers|float|sat_2019_ca|Number of Test Takers Grade 11|
|10|grade_11_erwb_bm_num|str|sat_2019_ca|The number meeting the Evidence-Based Reading & Writing (ERW) benchmark established by the College Board based on the New 2016 SAT test format as of March 2016 for Grade 11.|
|11|grade_11_erwb_bm_pct|str|sat_2019_ca|The percent of students who met or exceeded the benchmark for Evidence-Based Reading & Writing (ERW) test for Grade 11.|
|12|grade_11_erwb_maths_num|str|sat_2019_ca|The number of students who met or exceeded the benchmark for the New SAT Math test format as of March 2016 for Grade 11.|
|13|grade_11_maths_bm_pct|str|sat_2019_ca|The percent of students who met or exceeded the benchmark for SAT Math test for Grade 11.|
|14|grade_11_meet_bm_num|str|sat_2019_ca7|The total number of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math Grade 11.|
|15|grade_11_meet_bm_pct|str|sat_2019_ca|The percent of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math Grade 11.|
|16|grade_12_enroll|float|sat_2019_ca|Enrollment of Grade 12|
|17|grade_12_takers|float|sat_2019_ca|Number of Test Takers Grade 12|
|18|grade_12_erwb_bm_num|str|sat_2019_ca|The number meeting the Evidence-Based Reading & Writing (ERW) benchmark established by the College Board based on the New 2016 SAT test format as of March 2016 for Grade 12.|
|19|grade_12_erwb_bm_pct|str|sat_2019_ca|The percent of students who met or exceeded the benchmark for Evidence-Based Reading & Writing (ERW) test for Grade 12.|
|20|grade_12_maths_bm_num|str|sat_2019_ca|The number of students who met or exceeded the benchmark for the New SAT Math test format as of March 2016 for Grade 12.|
|21|grade_12_maths_bm_pct|str|sat_2019_ca|The percent of students who met or exceeded the benchmark for SAT Math test for Grade 12.|
|22|grade_12_meet_bm_num|str|sat_2019_ca|The total number of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math Grade 12.|
|23|grade_12_meet_bm_pct|str|sat_2019_ca|The percent of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math Grade 12.|

*sat_act_by_college*

|Field #|Field Name|Type|Dataset|Description|
|---|---|---|---|---|
|0|school|str|act_df|State in the US|
|1|test_optional|str|act_df|Whether SAT/ACT is option|
|2|applied_class_yr|str|act_df|Start year of policy|
|3|policy|int64|str|Policy of optional SAT/ACT|
|4|num_applicants|int64|act_df|Number of applicants for that university|
|5|acceptance_rate|float|act_df|Acceptance rate of university|
|6|sat_25|int64|float|25th percentile of accepted SAT score|
|7|sat_75|int64|float|75th percentile of accepted SAT score|
|8|act_25|int64|float|25th percentile of accepted ACT score|
|8|act_27|int64|float|75th percentile of accepted ACT score|
