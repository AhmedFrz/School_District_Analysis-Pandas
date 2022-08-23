# School_District_Analysis


### Overview of the school district analysis: Explain the purpose of this analysis.

Maria has been assigned the following task and we are to help her 
- To test the data for school district for analysis and give insights
- These insights will help in informed discussions and decision at strategic school district level 
- Analyze data on student funding, standardized tests
- Aggregate data and show trends in performance
- Then making decisions on school budget allocations


## Results: 

### How is the district summary affected?

old_district_summary_df

new_district_summary_df

### How is the school summary affected?
per_school_summary_df
per_school_summary_df


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
After removing the ninth graders' math and reading scores the average grades are not affected significantly


### How does replacing the ninth-grade scores affect the following:


### Math and reading scores by grade
reading_scores_by_grade
math_scores_by_grade


### Scores by school spending
spending_summary_df


### Scores by school size
size_summary_df


### Scores by school type
type_summary_df


### Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

Dealing with missing values is crucial and it may affect the analysis and may lead to wrong decisions. Ninth grader was replaced with Nans as this would not affected the summary because replacing it with zero will affect the average and would give incorrect average information

School ranking

Math and reading scores

Spending changes
