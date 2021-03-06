# 04_PyCitySchools_Challenge
School district Analysis using pandas and jupyter Notebook
## Overview of the school district analysis
The purpose of this analysis is to perform EDA and  determine the following metrics using pandas and Jupyter notebook. 
We are provided with two csv files that contain the school data (School name, type, size and budget) and student data (student_name,gender,grade,school name, reading and math scores of each student)

Key Metrics:
- A high-level snapshot of the district's key metrics.
- An overview of the key metrics for each school.
- Tables presenting each of the following metrics:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

It was then brought to attention that the math and reading grades of 9th grade students for Thomas high school appear to have altered. Hence an additional/updated analysis for the same metrics has to be performed by replacing the math and reading scores with NaNs for Thomas High School 9th grade students and keeping the rest of the data in tact
## Results
- How is the district summary affected?

Replacing the 9th grade data has not made a significant impact on the district summary as only 461 out of 39170 student’s scores has been excluded from calculations.

_Initial District Summary_
![](Images/District_Summary_Initial.png)
_Updated District Summary_
![](Images/District_Summary_Updated.png)


_District Summary Change_

![](Images/District_Summary_Comparison.png)

- How is the school summary affected?

The school summary is impacted  and dropped heavily for the % Passing Math, % Passing Reading, and % Overall Passing data  for Thomas High School as shown.

_Initial School Summary_

![](Images/School_Summary_Initial.png)

_Updated School Summary_

![](Images/School_Summary_Updated.png)

_School Summary Change_

![](Images/School_Summary_Comparison.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the initial analysis, we see that Thomas High School was second on the list when sorted by % Overall Passing. On Updated analysis, Thomas High school moved to  8th place based on % overall passing data.

_THS Updated Analysis_

![](Images/THS_Updated_Analysis.png)

- How does replacing the ninth-grade scores affect the following:

**Math and reading scores by grade**

The updated math and reading scores by grade  shows NaN for 9th grade Thomas High School Data

![](Images/Math_Scores_By_Grade.png)

![](Images/Reading_Scores_By_Grade.png)

**Scores by school spending**

Thomas High School falls under the category of spending range $631-645. We can observe very minimal/negligible impact on the data for the spending Range $631-645

_Initial School Spending_

![](Images/Spending_Summary_Initial.png)

_Updated School Spending_

![](Images/Spending_Summary_Updated.png)


**Scores by school size**

Thomas High School falls under the category of  school size “Medium” with a total of 1635 students. We can observe very minimal/negligible impact on the data for the “Medium” range schools student population

_Initial scores by size_

![](Images/Size_Summary_initial.png)

_Updated scores by size_

![](Images/Size_Summary_Updated.png)

**Scores by school type**

_Initial Scores by Type_

![](Images/SchoolType_Summary_initial.png)

_Updated scores by Type_

![](Images/SchoolType_Summary_Updated.png)


Both the initial analysis and updated analysis shows that Charter schools have a high overall passing percentage of around 90% whereas District schools around 54%.

## Summary: 

- The initial analysis showed  Thomas High School on the  second position when sorted by % Overall Passing. On Updated analysis, Thomas High school went to the 8th place based on % overall passing data. The overall passing% dropped from 91% to 65% for the school summary.
- Another updated school summary is data is produced after removing the 9th graders count from THS and recalculating the #% Passing Math,% Passing Reading and % Overall Passing based on 10th ,11th and 12th grade student counts from Thomas High School. The overall passing percent bumped to 90.630324 when calculated for 1174 students through grades 10, 11 and 12.
- The Math and Reading scores by grade shows the value Nan for 9th graders Thomas High School.
- The scores by school size or type shows no significant change when compared to initial analysis and updated analysis
-  An interesting observation is the student counts for district schools ( 26976) and charter schools (12194). We have the more than twice the data for district schools as compared to charter schools.


