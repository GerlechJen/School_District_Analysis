# School District Analysis

## Overview
A Chief Data Scientist for a city school district who is to analyze data on student funding and student’s standardized test scores, asked me to assist her. The results of the analysis will be made into a report and presented. The final presentation would provide insights about performance trends and patterns which will inform discussions and strategic decisions at the school and district level.

To perform this task, I had complete access to every student’s math and reading scores, as well as, other data on the schools they attend. I completed the analysis and showcased trends in school performance which helped the school board and superintendents to make decisions regarding the school budgets and priorities.

In this project, I have been asked to replace the math and reading scores for Thomas High School ninth graders with NaNs while keeping the rest of the data intact. Afterwards, I am to repeat the school analysis and write up a report to describe how these changes affected the overall analysis. These changes have been requested because there has been evidence of academic dishonesty in the reading and math grades of Thomas High School ninth graders.

## Results
* How is the district summary affected?

When the math and reading scores of 9th graders from Thomas High School was removed, the district summary results was impacted very slightly. There was a small change in the Average Math Score. It decreased from 79.0 to 78.9. Aside that, every other value in the district summary remained the same. 

The images below show the results of before and after the changes were made to the data respectively. 
 
 ![image1](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/old_district_summary.png)
 
 ![image2](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/new_district_summary.png)
 
 
* How is the school summary affected?

The school summary was greatly affected when the math and reading scores for 9th graders from Thomas High School was replaced with NaNs, but the total number of students in Thomas High School was still used in our calculations. For that scenario, the average math score decreased from 83.418349	to 83.350937. The percentage passing math decreased from 93.272171 to 66.911315. The percentage passing reading decreased from 97.308869 to 69.663609. The overall passing percentage decreased from 90.948012 to 65.076453. It was only the average reading score that saw an increase from 83.848930 to 83.896082. The image below shows the results after using the total number of students in Thomas High School for our calculations.

![image3](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/new_school_summary.png)

However, when the calculations were corrected taking into consideration just the 10th to 12th graders count of students, the average math score had the same changes with a decrease from 83.418349	to 83.350937. The percentage passing math had just a slight decrease from 93.272171 to 93.185690. The percentage passing reading decreased slightly too from 97.308869 to 97.018739. The overall passing percentage decreased just a little from 90.948012 to 90.630324 and the average reading score once again had an increase from 83.848930 to 83.896082. The corrected results is shown below:

![image4](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/corrected_school_summary.png)

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Before 9th grade math and reading scores was removed, Thomas High School was the second top performing school with overall passing percentage of 90.948012. After the changes were made and the averages calculated using just the 10th to 12th graders scores and population, Thomas High School was still the second top performing school but with a reduced overall passing percentage of 90.630324. The two different results are presented below:

![image5](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/old_top_schools.png)

![images6](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/new_top_schools.png)
  
* How does replacing the ninth-grade scores affect the following:
1. Math and reading scores by grade

With the exception of the math score of Thomas High School 9th graders that was changed from  83.6 to nan, the math scores by grades remained the same for the other schools. The reading scores also remained the same for the other schools while that of Thomas High School 9th graders changed from  83.7 to nan.
  
2. Scores by school spending

Looking at the overal spending summary dataframe,  the results of the students performance for the different spending ranges remained the same as when the 9th graders scores had not been removed. Therefore, replacing the ninth-grade scores did not have any impact on this result. 

![image7](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/scores_by_school_spending.png)

3.	Scores by school size

From the size summary dataframe, replacing the ninth-grade scores did not have any effect on the results as it remained the same. 

![image8](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/scores_by_school_size.png)

4. Scores by school type

The results in the scores by school type data frame remained the same which implies that replacing the ninth-grade scores had no effect on the previous results presented.

![image9](https://github.com/GerlechJen/School_District_Analysis/blob/main/images_folder/scores_by_school_type.png)

## Summary
After reading and math scores for the ninth grade students at Thomas High School were replaced with NaNs, these four changes were observed in the updated school district analysis: 
1. A new total student count of 38,709 was calculated and used for further calculations.
2. The number of 9th grade students in Thomas High School had to be deducted from the total number of students in the school before finding the passing math percentage, passing reading percentage and passing overall percentage of Thomas High School accurately. 
3. The dataframe showing the average math and reading scores by grade had the values for Thomas High School 9th graders represented by nan.
4. The loc method was very useful in this second analysis as it made it possible to select and alter specific parts of the data for analysis.

