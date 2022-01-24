# PyCity Schools District Analysis

## **Overview of PyCity School District Analysis**
The purpose of the PyCitySchools district analysis was to assess and analyze school performance of PyCity districts. Irregularities were observed among the Ninth Grade results for Thomas High School, and so these results were removed from the analysis. Schools were assessed in the following areas:
	
*  Top five performing schools based upon overall passing rates
*  Bottom five performing schools based upon overall passing rates
*  Average math score for each grade level from each school
*  Average reading score for each grade level from each school
*  Scores by school spending per student
*  Scores by school size
*  Scores by school type

Additionally, the effects of removing the St Thomas High School Ninth Grader data is sicussed, where relevant. All of these findings are discussed within the "PyCity School District Analysis Results" section below.

## **PyCity School District Analysis Results**

The results of the updated analysis are summarized in in *Figure 1* to *Figure 9*. Results are discussed below these figures.

![Figure 1](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/1_FinalDistrictSummary.png)
**_Figure 1_:** Schools Districts Summary

![Figure 2](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/2_FinalSchoolSummary.png)
**_Figure 2_:** Schools Summary

![Figure 3](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/3_FinalTopFive.png)
**_Figure 3_:** Top 5 schools, based on overall passing rate

![Figure 4](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/4_FinalBottomFive.png)
**_Figure 4_:** Bottom 5 schools, based on overall passing rate

![Figure 5](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/5_AverageMath.png)

**_Figure 5_:** Average math score, for each grade level for each school

![Figure 6](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/6_AverageReading.png)

**_Figure 6_:** Average reading score, for each grade level for each school

![Figure 7](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/7_FinalScoreBySchoolSpending.png)
**_Figure 7_:** Scores by school spending per student

![Figure 8](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/8_FinalScoreBySchoolSize.png)
**_Figure 8_:** Scores by school size

![Figure 9](https://github.com/CR-HSDC/School_District_Analysis/blob/main/resources/9_FinalScoreBySchoolType.png)
**_Figure 9_:** Scores by school type

### **How is the district summary affected?**

Per *Figure 1* the average math score (79.0 vs. 78.9%), % Passing Math Score (75% vs 74.8%), % Passing Reading (86 vs. 85.7%) and % Overall Passing Score (65 vs. 64.9% scores are affected).

***Student Note 1:***  *It is unclear from the provided notes, and starting code if the updated student count should be used throughout. If so, this will lead to inaccurate statistics (e.g. total budgets would be calculated based on all students, but student count would be less the Thomas High Ninth Graders). For example in cell 7 of the starting code the following code is provided, which is not listed as a required step:*

### **total-budget = school-data-df["budget"].sum()**

*This will calculate the budget for all students. For this reason and to provide meaningful results, the total student count for Thomas High School is used. Otherwise there is the potential for confusion and inaccurate results. Cell 13 of the starting code, which assembles the district_summary_df dataframe inserts the total_budget based on all students, and use the student_count variable. For this reason the total student count (including Thomas High School Ninth graders) was used, and all results discussed herein reflect that. For the purposes of calculating math/reading avreage the adj_student_count variable was used and is available for viewing in the PyCitySchools_Challenge source code*

### **How is the school summary affected?**

Per *Figure 2* the Average Math and Readings Scores and % Passing Math, % Passing Reading and % Overall Passing scores are affected for Thomas High Scores. Results are shown on *Figure 2* and the affected results highlighted in red.

### **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools**

Per *Figure 3* the overall ranking of Thomas High School was unchanged from its original position. The Average Math, Reading, % Passing Math, % Passing Reading and % Overall Passing Scores changed slightly as highlighted by red boxout on *Figure 3*

### **How does replacing the ninth-grade scores affect Math & Reading Score by grade?**

Per *Figure 4* and *Figure 5* there are no ninth grade scores for Thomas High School. "NaN" is shown for these results, this is due to all values being replaced by the numpy.nan() value. Calculations and analysis were not performed on these values.
This does not affect any of the other schools, or grades in this analysis.

### **How does replacing the ninth-grade affect scores by school spending?**

Per *Figure 7* average math and reading scores, and % Passing Math, % Passing Reading and % Overall Passing Scores were slightly affected, as highlighted by red boxout on *Figure 7*

See **Student Note 1** above as it relates to these results; this table considered the total student count and budget, based upon the rationale outlined in that note.

### **How does replacing the ninth-grade affect scores by school size?**

Per *Figure 8* scores by school size were unaffected by the updated analysis.

### **How does replacing the ninth-grade affect scores by school type?**

Per *Figure 9* scores by school type were unaffected by the updated analysis.


## **PyCity School District Analysis Summary**

From the above analysis, it can be seen that Average Math Score, Average Reading Score, % Passing Math, % Passing Reading and % Overall Passing were affected by the updated PyCity Schools analysis. The removal of the Thomas High School ninth grade results was responsible for this change. Results are summarized in *Figure 7* and the affected results highlighted by red boxout.
	






