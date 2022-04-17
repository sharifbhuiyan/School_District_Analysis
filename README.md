## **<h1 align="center"> School_District_Analysis**




  ## Overview of the school district analysis: 
<p align="justify">Reviewing the previous analysis, school board has identified something anomaly in source file, students_complete.csv. Authority noticed an evidence of academic dishonesty. Specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Now new analysis has been furnished by replacing the math and reading scores for Thomas High School with NaNs and keeping the rest of the data intact. <p>

<p align="justify">This new analysis consists of two technical analysis.<p>

  - Replace ninth-grade reading and math scores
  - Repeat the school district analysis

 
  School district analysis PyCitySchools_Challenge.ipynb file link -  [ School district analysis](https://github.com/sharifbhuiyan/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)  

  
- Resources :
  - Data source : schools_complete.csv, students_complete.csv
  - Software : Pandas library, Jupyter Notebook


  
  
 ## School district analysis Results: 
  
<p align="justify"> The following metrics are recreated to repeat the school district analysis : 


- The district summary
- The school summary
- The top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score for each grade level from each school
- The average reading score for each grade level from each school
- The scores by school spending per student, by school size, and by school type
 <p>
  
   <p align="justify">•	The district summary has been changed after replacing the 9th grade students of Thomas High School. Previously Overall passing rate was 65.2, present rate is 64.9. It can be visualized by following snapshot. <p>
  
  Updated :   
<p align="center">
  <img width="500" src=https://github.com/sharifbhuiyan/Election_Analysis/blob/main/Resources/Anlysis_3.png
</p>
  
  Previous : 
<p align="center">
  <img width="500" src=https://github.com/sharifbhuiyan/Election_Analysis/blob/main/Resources/Anlysis_3.png
</p>
  

  <p align="justify">•	•	The school summary of Thomas High school has beenc hanged after replacing the 9th grade students of Thomas High School. Previously Overall passing rate was 65.07, present rate is 90.63. It can be visualized by following snapshot. <p>
  
  Updated :   
<p align="center">
  <img width="500" src=https://github.com/sharifbhuiyan/Election_Analysis/blob/main/Resources/Anlysis_3.png
</p>
  
  Previous : 
<p align="center">
  <img width="500" src=https://github.com/sharifbhuiyan/Election_Analysis/blob/main/Resources/Anlysis_3.png
</p>
   
  
  
 The command To select all the reading scores from the 9th grade at Thomas High School and replaced them with NaN is : 
 
```ruby
    
    txt_file.write(winning_candidate_summary)

```
  

  The commmand to replace the overall passing percentage for Thomas High School in the per_school_summary_df  iss : 
 
```ruby
    
    txt_file.write(winning_candidate_summary)

```

  
  
  
  
  
  Command for Save the winning candidate's summary to the text file :
  ```ruby
    
    txt_file.write(winning_candidate_summary)

```
  
    
 Command for print the winning candidate to terminal :

  
 ```ruby
    winning_candidate_summary = (
        f"-------------------------\n"
        f"Winner: {winning_candidate}\n"
        f"Winning Vote Count: {winning_count:,}\n"
        f"Winning Percentage: {winning_percentage:.1f}%\n"
        f"-------------------------\n")
    print(winning_candidate_summary)
    
  ```
  
  
 ### Election-Audit analysis outcomes were :

- Total  369,711 votes were cast in this congressional election.

- The number of votes and the percentage of total votes casted for each county was :
 
 <p align="center">
   
| 	County  | % of casting vote  | Casting vote |
| :------------ |:---------------:| -----:|
| Jefferson      | 10.5% | 38,855 |
| Denver      | 82.8%        |   306,055 |
| Arapahoe | 6.7%        |    24,801 |

</p>
   
   
- The county, Denver had the largest number of votes, 306,055.

- The number of votes and the percentage of the total votes each candidate received :

| 	Candate  | Number of received votes  | % of received vote |
| :------------ |:---------------:| -----:|
| Charles Casper Stockham      | 85,213 | 323.0% |
| Diana DeGette      | 272,892        |   73.8% |
| Raymon Anthony Doane | 11,606        |    3.1% |
  
- Diana DeGette won the election. The number of received votes was 272,892 and percentage of the total votes was  73.8%.
  
  
 

    
    
    
    
## School district analysis Summary:
  <p align="justify">Finally, school district analysis have been updated after replacing  the reading and math scores for the ninth grade at Thomas High School with NaNs.

•	The district summary affected by replacing the 9th grade students of Thomas High School.

•	How is the school summary affected?


•	How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
•	How does replacing the ninth-grade scores affect the following:

Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type

<p>
  
<p align="justify">Suppose for city election, need to change the all county tracking code. Like : <p>

- Have to remove the code for tracking the largest county and county voter turnout.
```ruby   
county_name = ""
county_voting = 0
```
  
  - Have to remove the code for printing the largest turnout county.
  
  ```ruby   
    winning_county_summary = (
    f"-------------------------\n"
    f"Largest County Turnout: {c_winning_county}\n"
    # f"Winning Vote Count: {c_winning_count:,}\n"
    # f"Winning Percentage: {c_winning_percentage:.1f}%\n"
    f"-------------------------\n")
    print(winning_county_summary)
