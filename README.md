# School_District_Analysis

## Project Overview
This is a statistical analysis of a local city school district's standardized testing and student funding. The analysis is being conducted for the school district's school board to inform them on trends on student performance and student funding to enable them to make informed budgeting decisions.  An original analysis was conducted with the given data and then evidence of academic dishonesty was discovered within the Thomas High School ninth graders' scores.  A second analysis was conducted with the Thomas High School ninth graders' math and reading scores replaced with NaN values, or not a number. The second analysis coducted will be referred to as the adjusted analysis.  The required tasks for the analysis are listed below:

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
- The original school district summaryis shown below:

![district_summary_df]()

- The original by-school summary is shown below:

![school_summary_df]()

- The original top 5 performing schools are:

![high_5]()

- The original bottom 5 performing schools are:

![low_5]()

- The original average math scores by grade are:

![math_scores_by_grade]()

- The original average reading scores by grade are:

![reading_scores_by_grade]()

- The original average scores by spending per student are:

![scores_by_per_student_spending]()

- The original average scores by school size are:

![scores_by_school_size]()

- The original average scores by school type are:

![scores_by_school_type]()


### Adjusted Analysis
To conduct the adjusted analysis, the Thomas High School ninth graders' math and reading scores were replaced with NaN values, or not a number. A 'loc' script was used to filter just the scores from the Thomas High School ninth graders:

![loc_script_replacing_scores_with_NaNs]()

The resulting student data with the replaced scores shows NaN values in the Thomas High School ninth graders' scores:

![student_data_df_after_NaNs]()

- The adjusted school district summaryis shown below:

![district_summary_df_NEW]()

- The adjusted by-school summary is listed below:

![school_summary_df_NEW]()

- The adjusted top 5 performing schools are:

![high_5_NEW]()

- The adjusted bottom 5 performing schools are:

![low_5_NEW]()

- The adjusted average math scores by grade are:

![math_scores_by_grade_NEW]()

- The adjusted average reading scores by grade are:

![reading_scores_by_grade_NEW]()

- The adjusted average scores by spending per student are:

![scores_by_per_student_spending_NEW]()

- The adjusted average scores by school size are:

![scores_by_school_size_NEW]()

- The adjusted average scores by school type are:

![scores_by_school_type_NEW]()

## School District Analysis Summary
4 changes in the updated school district analysis after Thomas HS 9th reading and math scores replaced with NaNs