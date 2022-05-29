# School_District_Analysis

## Overview of the School District Analysis
A Chief Data Scientist for a city school district who is to analyze data on student funding and student’s standardized test scores then make a report and presentation, asked me to assist her. The final presentation to be made would provide insights about performance trends and patterns which will inform discussions and strategic decisions at the school and district level.
To perform this task, I had complete access to every student’s math and reading scores, as well as, other data on the schools they attend. I completed the analysis and showcased trends in school performance which helped the school board and superintendents to make decisions regarding the school budgets and priorities
In this project, I have been asked to replace the math and reading scores for Thomas High School ninth graders with NaNs while keeping the rest of the data intact. Afterwards, I am to repeat the school analysis and write up a report to describe how these changes affected the overall analysis. These changes have been requested because there has been evidence of academic dishonesty in the reading and math grades of Thomas High School ninth graders.

# Results: Using bulleted lists and images of DataFrames as support, address the following questions.
* How is the district summary affected?

 When the math and reading scores for 9th graders from Thomas High School was removed, the district summary results was impacted very slightly. There was a small change in the Average Math Score. It decreased from 79.0 to 78.9. Aside that, every other value in the district summary remained the same. 
 
* How is the school summary affected?

The school summary was greatly affected when the math and reading scores for 9th graders from Thomas High School was removed. The average math score decreased from 83.418349	  to 83.350937. Average reading score increased from 83.848930 to 83.896082. The percentage passing math decreased from 93.272171 to 66.911315. The percentage passing reading decreased from 97.308869 to 69.663609. The overall passing percentage decreased from 90.948012 to 65.076453.

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Before 9th grade math and reading scores was removed, Thomas High School was the second top performing school with overall passing percentage of 90.948012. After the changes were made, Thomas High School was still the second top performing school but with a reduced overall passing percentage of 90.630324.
  
* How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade

With the exception of the math and reading scores of Thomas High School 9th graders that was changed from  83.6 and 83.7 respectively to nan, the math and reading  scores by grades remained the same for the other schools.
  
- Scores by school spending
For the scores by school spending, the average math score, average reading score, percentage passing math, percentage passing reading and the overall passing percentage reduced for Thomas High School when the ninth-grade scores were replaced with nan. 
But the overal size spending summary data frame remained the same. 

-	Scores by school size
With the exception of the average reading score of Thomas HighSchool that increased by school size.
But the overal size summary data frame remained the same. 

-	Scores by school type
The scores by school type remained the same.

The output is shown in the image below:


# Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.


