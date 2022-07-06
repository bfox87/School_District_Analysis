# School District Analysis

## Overview:
### Background:
Maria, the chief data scientist for City School System, is needing assistance in analyzing school funding and standardized test data. The task is to aggregate the data to showcase trends in school performance. This will in turn help the school board and superintendent make decisions regarding school budgeting allotments. To further complicate matters, the school board believes there is evidence of academic dishonesty with the ninth grade reading and math scores at Thomas High School.

### Purpose:
The purpose of this project is to cleanse the dataset of the potentially altered reading and math grades at Thomas High School by replacing these scores with null or NaN values. Then we will repeat the school district analysis done earlier. Any changes to results will then be noted.

## Results:
- **DISTRICT SUMMARY EFFECTS**:
    - The large size of the school district at 39,170 students makes the effects of removing of 461 ninth grade math and reading scores at Thomas High fairly small.
    - The average math score dropped slightly from 79.0 to 78.9 while the reading score change was too small to register at one decimal place.
    - The pass rates did drop with the removal of the Thomas ninth grade scores. However, these drops were quite small due to the dilution within the large district.
        - % Passing Math: 75.0 down to 74.8
        - % Passing Reading: 85.8 to 85.7
        - % Passing Overall: 65.2 to 64.9
    - **Before replacement**:
     
    ![District_Summary_before_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/District_Summary_before_replace.PNG)
    
    - **After replacing ninth grade scores**:
    
    ![District_Summary_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/District_Summary_after_replace.PNG)
    
- **SCHOOL SUMMARY EFFECTS**:
    - The removal of all ninth grade math and reading scores at Thomas High caused a drop of between 26-27% in math, reading, and overall pass rates at the school. No other school's results were affected.
        - % Passing Math: 93.3 down to 66.9
        - % Passing Reading: 97.3 to 69.7
        - % Passing Overall: 90.9 to 65.1
    - Thomas High average reading score dropped slightly from 83.42 to 83.35. The average math score went up slightly from 83.85 to 83.9.
        - The average math and reading scores of the remaining 10th through 12th graders at Thomas High was very close to that of the removed ninth graders. This is why the average scores for the school changed only slightly.
    - **Before replacement**:
     
    ![School_Summary_before_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Summary_before_replace.PNG)
    
    - **After replacement**:
    
    ![School_Summary_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Summary_after_replace.PNG)

- **THOMAS HIGH SCHOOL RELATIVE PERFORMANCE CHANGES**:
    - As seen in the screenshots above, before the exclusion of ninth grade test results, Thomas High's overall pass rate of 90.9% was good enough for second best in the district. With removal of the ninth grade reading and math scores, the school drops to eighth place with a 65.1% overall passing rate.
    
- **EFFECT ON MATH AND READING SCORES BY GRADE**:
    - A null or "nan" value is now present for Thomas High ninth grade reading and math scores.
    - The only scores affected by removal are the ninth grade scores at Thomas High. All other schools for ninth grade are unaffected as are the 10th-12th grade scores at all schools, including Thomas High.
    - **After replacement for on math scores (no reading screenshot to save space)**:

![School_Grade_Scores_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Grade_Scores_after_replace.PNG)

- **EFFECT ON SCORES BY SCHOOL SPENDING**:
    - Thomas High has a budget per student of $638 ($1,043,130 budget / 1,635 students). Therefore, the schools falls into the $631-$645 spending bin. As such, changes are only seen in this spending category. 
    - Around a seven point drop in the percentage of students passing is seen:
        - % Passing Math: 73 down to 67
        - % Passing Reading: 84 to 77
        - % Passing Overall: 63 to 56
     - Changes in avg reading/math scores too small to register with the rounding to one decimal place.
     - **Before replacement**:
     
    ![School_Spending_Scores_before_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Spending_Scores_before_replace.PNG)
    
     - **After replacement**:
    
    ![School_Spending_Scores_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Spending_Scores_after_replace.PNG)
    
- **EFFECT ON SCORES BY SCHOOL SIZE**:
    - With 1,635 students, Thomas High falls into a Medium school size so changes only seen in this category.
    - Around a six point drop in the percentage of students passing math, reading, and both:
        - % Passing Math: 94 down to 88
        - % Passing Reading: 97 to 91
        - % Passing Overall: 91 to 85
     - Changes in avg reading/math scores too small to register with the rounding to one decimal place.
     - **Before replacement**:
     
    ![School_Size_Scores_before_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Size_Scores_before_replace.PNG)
    
    - **After replacement**:
    
    ![School_Size_Scores_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Size_Scores_after_replace.PNG)
    
- **EFFECT ON SCORES BY SCHOOL TYPE**:
    - Thomas High is categorized as a Charter school so changes only seen in this row.
    - Close to a four point drop in the percentage of students passing math, reading, and both:
        - % Passing Math: 94 down to 90
        - % Passing Reading: 97 to 93
        - % Passing Overall: 90 to 87
     - Changes in avg reading/math scores too small to register with the rounding to one decimal place.
     - **Before replacement**:
     
    ![School_Type_Scores_before_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Type_Scores_before_replace.PNG)
    
    - **After replacement**:
    
    ![School_Type_Scores_after_replace](https://github.com/bfox87/School_District_Analysis/blob/main/Resources/Screenshots/School_Type_Scores_after_replace.PNG)

## Summary:
To begin, replacing Thomas High ninth grade math and reading scores with NaN's caused pass rates to decline (% passing math, % passing reading, and & passing both/overall). The rate of decline depended on the size of the analysis. Looking at large categories like the entire district or by school type, the effect was diluted by all the other student/school scores that were never changed. The drop in pass rates is more pronounced when there is a smaller dataset. **Secondly**, when comparing against other schools, this decline in overall pass rates caused Thomas High School to drop dramatically in the rankings, from second place in the district to eighth. This change from one of the top schools to middle of the pack could have dramatic impacts on the school going forward. **Third**, the average test scores did not change by much, even when looking at just Thomas High alone. This is because the test scores for Thomas' 10th - 12th grades were very similar to those of the removed ninth graders. **Finally**, we could replace the Thomas ninth grade NaN's with the school's 10th -12th grade results (done at end of ipynb file). Including potentially dishonest ninth grade results is not advised, but replacing with null values makes the school's pass rates look worse than they really are. Using these 10th - 12th grade results instead accomplishes the goal of removing potentially corrupt data, but keeps the pass rates near where they likely would be if ninth grade was valid. 
