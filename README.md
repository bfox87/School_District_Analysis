# School District Analysis

## Analysis Overview:
### Background:
Maria, the chief data scientist for City School System, is needing assistance in analyzing school funding and standardized test data. The task is to aggregate the data to showcase trends in school performance. This will in turn help the school board and superintendent make decisions regarding school budgeting allotments. To further complicate matters, the school board believes there is evidence of academic dishonesty with the nineth grade reading and math scores at Thomas High School.

### Purpose:
The purpose of this project is to cleanse the dataset of the potentially altered reading and math grades at Thomas High School and then repeat the school district analysis done earlier. Any changes to results will then be noted.

## Results:
- District Summary Effects:
    - Jefferson: 38,855 votes (10.5% of total)
    - Denver: 306,055 votes (82.8% of total)
    - Arap
- School Summary Effects:
    - Jefferson: 38,855 votes (10.5% of total)
    - Denver: 306,055 votes (82.8% of total)
    - Arapahoe: 24,801 votes (6.7% of total)
- Thomas High School relative peformance changes:
    - Vote count: 272,892
    - Perc
- Effect on math and reading scores by grade:
    - Charles Casper Stockham: 85,213 votes (23.0% of total)
    - Diana DeGette: 272,892 votes (73.8% of total)
    - Raymon Anthony Doane: 11,606 votes (3.1% of total)
- Effect on scores by school spending:
    - Vote count: 272,892
    - Percentage of total votes: 73.8%
- Effect on scores by school size:
    - Vote count: 272,892
    - Percentage of total votes: 73.8%
- Effect on scores by school type:
    - Thomas High is categorized as a Charter school so changes only see in this row.
    - Close to a four point drop in the percentage of students passing math, reading, and both
        - % Passing Math: 94 down to 90
        - % Passing Reading: 97 to 93
        - % Passing Overall: 90 to 87
     - Before replacement:
    ![Terminal_Output](https://github.com/bfox87/Election_Analysis/blob/main/analysis/Terminal_Output.PNG)
    - After replacing nineth grade scores:
    ![Terminal_Output](https://github.com/bfox87/Election_Analysis/blob/main/analysis/Terminal_Output.PNG)


The results above have been printed to a text file in the analysis folder, but a screenshot of the Python terminal output has been pasted below for confirmation:



## Summary:

To begin, Secondly. Third. Fourth and finally, his Python script has resulted in an accurate, efficient audit of this precinct's congressional election results. However, the real benefit will come from its use in future elections. The script can be modified to summarize results in a variety of different ways, as detailed below.

#### Snippets of code needed for future uses:
- In either of these examples, the original Python code can be adjusted. To begin, an analyst will need to initialize an empty list and dictionary to hold the names (i.e. precinct or vote method) and votes cast as values. Example code pasted below is from the county analysis. 
```
# Create a county list and county votes dictionary.
county_options = []
county_votes = {}
```

