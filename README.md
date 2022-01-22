# PyCity School District Analysis

## Overview of the school district analysis: 
### Project Goals:
- This data analysis aims to provide a comprehensive look at funding, student performance, and school size for the high schools in the PyCity school district.
- This analysis aims to assist the school board in comparing the effects of school funding, size, and type on student performance. 
- This report aims to direct the school board toward trends appearing within the PyCity high schools. 

### Important Steps in the overall Data Analysis: 
- Cleaning the data: 
	- Some student names had been entered incorrectly. In order to correct our records, it was necessary to clean this data.
- Creating data frames: 
	- Throughout the data analysis, you should see charts called, "data frames." These data frames allow you to see a variety of information about the high schools including:
		- complete student data
		- complete school data
		- a summary of ninth grade performance throughout the district
		- a comparison of how schools perform based on their funding
		- and more
- Merging school and student data: 
	- For a more complete analysis, it was necessary to merge the school and student data.
	- This allowed the analysis to examine the qualities of each school that may contribute to student success or failure. 


## Results
Due to the investigation of ninth grade reading and math scores from Thomas High School, this document presents both the original data frames (including Thomas High School ninth grade scores) and the refactored data frames (in which those scores have been excluded).

- How is the district summary affected by the removal of THS reading and math scores?
	- See the image below for the original district summary: 
		-  ![original_district_summary](https://user-images.githubusercontent.com/93888037/150654737-14a0f57d-146a-4b75-b2f3-02eaeb8a5bff.png)

	- Here is the district summary with the THS ninth grade scores removed:
		-  ![minusths_district_summary](https://user-images.githubusercontent.com/93888037/150654751-a40a4152-5dd7-4f79-bf49-e004aa9b78e0.png)

	- These images show a slight change in the numbers caused by the removal of the THS reading and math scores.
		- the Average Reading percentage, the percent of students passing math, the percent of students passing reading, and the overall passing percentage were all raised by nearly one point once the THS scores had been removed. 

- How is the school summary affected?

	- Since only one school was affected by this investigation, the school summary shows very little change from the original version of the code to the modified code.
	- The only changes can be found in the Thomas High School row, which will be discussed in the next section of the summary. 
	

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
	- Because the numbers for Thomas High School did not change drastically with or without the ninth grade scores, the affect on the overall school summary is minimal.
		- After the removal of ninth grade numbers, THS remains in the top five schools in the district, and remains the second-highest school in the district when ranked by the overall percentage of students who passed.
		- However, you can see in these two images that the percentages of students passing math, students passing reading, and overall passing percentage were raised slightly when ninth grade scores were included.
			- Original Data Analysis for THS:
				- ![original_school_summary](https://user-images.githubusercontent.com/93888037/150654774-7142c4cc-a90b-4741-a72f-f1cb2b467f1f.png)
			- Modified Data Analysis for THS: 
				- ![minusths_school_summary](https://user-images.githubusercontent.com/93888037/150654782-6f863baa-ea27-4481-a46f-1f33bbb9aa8d.png)


- How does replacing the ninth-grade scores affect the following:
	- Math and reading scores by grade
		- Below you will see the data frames for the original math scores, and the modified math scores, sorted by grade:
			- Original Math Scores by Grade
				- ![original_math_scores_by_grade](https://user-images.githubusercontent.com/93888037/150654827-7243d8ef-903e-47a6-8731-81de51962200.png)
			- Modified Math Scores by Grade
				- ![minusths_math_scores_by_grade](https://user-images.githubusercontent.com/93888037/150654836-b0735856-9d86-40eb-aae5-a72c8db4a2ca.png)

		- Below you will see the data frames for the original reading scores, and the modified reading scores, sorted by grade:
			- Original Reading Scores by Grade
				- ![original_reading_scores_by_grade](https://user-images.githubusercontent.com/93888037/150654846-6126517d-723c-493d-a9d9-2bfa80da0566.png)
			- Modified Reading Scores by Grade
				- ![minusths_reading_scores_by_grade](https://user-images.githubusercontent.com/93888037/150654874-6ce9bbd3-7cb3-4a18-841f-e4687b756cf8.png)


		-In both cases, the other schools were not affected, but you can see where the "NaN" or "N/A" has been put in for the THS ninth grade scores.

	- Scores by school spending
		- Below you will see the original scores, broken down to their school spending per capita: 
      - ![original_scores_by_spending_hl](https://user-images.githubusercontent.com/93888037/150654924-e61652ad-d1de-4ed6-8229-f563c9bc2b6f.png)
    - Here is the same break down, with the THS ninth graders removed:
			- ![minusths_scores_by_spending](https://user-images.githubusercontent.com/93888037/150654909-8c7374b4-0cb0-4acb-877c-d83d43cad855.png)

		- A very minute change can be spotted between these two data frames. With the exclusion of the THS ninth grade data, we can see that their spending level receives slightly different scores.
			- The percent of students passing math in the original data frame would round to 74%, while in the modified data frame it is only 73%.
			- Due to the relatively small number of students affected by the grade removal, the data stays virtually the same in each analysis.

	- Scores by school size
		- Similarly to scores by school spending, the removal of the ninth grade scores from THS has little to no affect on the analysis of student success based on school size.
		- These are the results showing student success by school size (from the modified version of the analysis):
			- ![scores_by_school_size_final](https://user-images.githubusercontent.com/93888037/150654934-70b91d86-49d5-43e6-af80-59cb1f2d311e.png)

	- Scores by school type
		- Again, scores by school type were not altered enough to affect the overall data analysis. 
		- Here are the results showing student success by school type (from the modified version of the analysis):
			- ![scores_by_school_type_modified](https://user-images.githubusercontent.com/93888037/150654941-bec18d35-5dd6-4ecc-86b3-eda310c7c049.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
- The primary changes found in the data after the removal of THS ninth grade scores is in THS's own data. 
- You can see that the removal of ninth grade THS scores affected the average reading score for Thomas High. 
- Additionally, the percentage of students passing math, passing reading, and passing both math & reading were raised by a percentage point when ninth grade data was removed.
- Finally, this removal greatly affects our ability to compare student success by grade level. 
	- Since an entire grade level had to be removed, this makes our analysis by grade level more difficult to process. 
	- The analysis of success by grade level should be set aside until clearer answers are available on the ninth grade scores from THS. 

