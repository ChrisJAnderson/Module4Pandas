# Module4Pandas
## Purpose of the Analysis
This analysis seeks to address the changes in school district metrics after removing scores subject to academic dishonesty in order to paint a more accurate picture of student performance within the districts. We use the python libraries numpy and pandas to accomplish this.
## Analysis
In order to obtain stats for comparison, I ran the program again without removing thomas high school's 9th grade scores, and was surprised at the small size of the difference.  
Here are the school district's stats before removing the dishonest scores:  
![](https://github.com/ChrisJAnderson/PyCitySchoolsChallenge/blob/main/images/schoolstatswithoutcleaning.png)  
And here are the stats afterwards:  
![](https://github.com/ChrisJAnderson/PyCitySchoolsChallenge/blob/main/images/schoolstatswithcleaning.png)  
-The total students metric is of course unchanged- the students are still there, their scores just don't count.  
-Same for the budget. Schools are still spending the same money on these students, even though they're cheating.  
-Average math score goes down by .1 after removing the offending class' scores. 
-Average reading score remains the same- we have more students passing reading than math, maybe the relatively small impact shown on the rest of the dataframe wasn't enough to affect this average significantly.  
-the percentage of students passing math drops by .2 after removing the cheaters.  
-The percentage of students passing reading also drops slightly (85.8 to 85.7 percent )after removing the grade 9 class at Thomas High School- proof that we have done something with it, although average reading score hasn't changed.  
-Our overall passing percentage drops by a staggering .3%, from 65.2% down to 64.9%.  
-In an effort to explain the relatively small impact of removing an entire class, I went to look at the population of Thomas High Scool versus the rest of the district. Thomas High has only 1635 students, and only 461 students in their grade 9 versus the total students in the district of 39,170. Removing their grade 9 scores has little impact on the district because of the small size of their grade.
## Summary
In summary, we can see that four scores- average math score, percent passing math, percent passing reading, and students passing overall, have been lowered by a very small amount. Average math scores drop by .1%, the percentage of students passing math drops by .2%, the percentage of students passing reading drops by .1%, and the percentage passing overall drops by .3%.  
However, Thomas High School's 9th grade is small enough that the academic dishonesty didn't have an outsized effect on their district metrics.
