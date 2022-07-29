# School_District_Analysis

## Project Overview
This is a statistical analysis of a local city school district's standardized testing and student funding. The analysis is being conducted for the school district's school board to inform them on trends on student performance and student funding to enable them to make informed budgeting decisions.  An original analysis was conducted with the given data and then evidence of academic dishonesty was discovered within the Thomas High School ninth graders' scores.  A second analysis was conducted by replacing the Thomas High School ninth graders' math and reading scores with NaN values, or not a number using the `loc` [method](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.loc.html). The second analysis coducted will be referred to as the adjusted analysis.  The required tasks for the analysis are listed below:

1. Develop a school district analysis summary with the following metrics:
    - Provide the total number of schools in the school district.
    - Provide the total number of students in the school district.
    - Provide the total budget for the school district.
    - Calculate the average math score for the school district.
    - Calculate the average reading score for the school district.
    - Calculate the percentage of students passing math for the school district.
    - Calculate the percentage of students passing reading for the school district.
    - Calculate the overall percentage of students passing both math and reading for the school district.
2. Develop a by-school analysis summary with the following metrics for each school:
    - Provide a listing of each school in the school district.
    - Provide the school type, charter or district for each school.
    - Provide the total number of students for each school.
    - Provide the total school budget for each school.
    - Calculate the average math score for each school.
    - Calculate the average reading score for each school.
    - Calculate the percentage of students passing math for each school.
    - Calculate the percentage of students passing reading for each school.
    - Calculate the overall percentage of students passing both math and reading for each school.
3. Calculate the top 5 performing schols based on the overall passing rate.
4. Calculate the bottom 5 performing schols based on the overall passing rate.
5. Calculate the average math score for each grade level from each school.
6. Calculate the average reading score for each grade level from each school.
7. Calculate the scores by school spending per student.
8. Calculate the scores by school size.
9. Calculate the scores by school type.

## Resources
- Data Source: schools_complete.csv and students_complete.csv
-  Software: Python 3.7.6, Anaconda 4.13.0, Visual Studio Code, 1.68.1

## School District Analysis Results
The analysis of the school district and their standardized testing returned the following results:
### Original Analysis
- The original school district summary is shown below:

![district_summary_df](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/district_summary_df.png)

- The original by-school summary is shown below:

![school_summary_df](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/school_summary.png)


### Adjusted Analysis
To conduct the adjusted analysis, the Thomas High School ninth graders' math and reading scores were replaced with NaN values, or not a number. A `loc` [script](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.loc.html) was used to filter just the scores from the Thomas High School ninth graders:

![loc_script_replacing_scores_with_NaNs](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/loc_script_replacing_scores_with_NaNs.png)

The resulting student data with the replaced scores shows NaN values in the Thomas High School ninth graders' scores:

![student_data_df_after_NaNs](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/student_data_df_after_NaNs.png)

- The adjusted school district summary is shown below:

![district_summary_df_NEW](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/district_summary_df_NEW.png)

- The adjusted by-school summary is listed below:

![school_summary_df_NEW](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/school_summary_NEW.png)

### Adjusted Results
The adjusted analysis returned the following results:
- Top 5 performing schools: The top 5 performing schools remained the same, but Thomas High School's score averages and percentages changed slightly, however Thomas High School still remained the number 2 performing school.
    1. Cabrerra High School
    2. Thomas High School
    3. Griffin High School
    4. Wilson High School
    5. Pena High School
- Bottom 5 performing schools: No change to the bottom 5 performing schools.
    1. Rodriguez High School
    2. Figueroa High School
    3. Huang High School
    4. Hernandez High School
    5. Johnson High School    
- Average math score for each grade level: The Thomas High School ninth 9th grade score changed to NaN.
- Average reading score for each grade level: The Thomas High School ninth 9th grade score changed to NaN.
- Average scores and percentage passing by school spending per student: no significant change.
- scores by school size: no significant change.
- scores by school type: no significant change.


## School District Analysis Summary
After updating the school district analysis to account for the adjusted Thomas High School 9th graders' reading and math scores replaced with NaNs, the changes to the scores did not make a significant impact on the overall analysis as even whith the adjusted scores Thomas High School still performed as the number 2 top performing school, but here are four changes to highlight:
   - The Thomas High School average math score decreased from 83.41 to 83.35 and the % of Thomas High School students passing math decreased from 93.27% to 93.18%.
   - The Thomas High School average reading score increased from 83.84 to 83.89 however the % of Thomas High School students passing reading decreased from 97.30% to 97.02%.
   - Thomas High School's overall percentage of students passing both math and reading decreased from 90.94% to 90.63%.
   - The math and reading scores by grade show a NaN value for the Thomas High School 9th grade column when compared to the other schools:
   
   Math Scores By Grade:
   
   ![math_scores_by_grade_NEW](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/math_scores_by_grade_NEW.png)

   Reading Scores By Grade:
   
   ![reading_scores_by_grade_NEW](https://github.com/mewers2/School_District_Analysis/blob/main/Resources/reading_scores_by_grade_NEW.png)
