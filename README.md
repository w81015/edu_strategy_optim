[中文版 Chinese version](README_zh.md)

# Educational Strategy Optimization and Reading System Efficacy Evaluation
- Analysis Subject: The reading performance of the same group of students over two consecutive years
- Objective: Propose (1) adjustments to teaching strategies; (2) optimizations for the reading system usage based on reading performance

## I. Process Description
1. Import data from 2020 (two datasets) and 2021 (two datasets), clean and merge them, then make preliminary observations (Python code).
2. Produce visual results with Power BI (Power BI dashboard).
3. Present analysis highlights and proposals with a presentation (presentation file).

## II. Data Description
1. Original Data:
    `df2020` contains all data from 2020 (consisting of df1 and df2), names not yet processed (cannot be disclosed).
2. Original Data:
    `df2021` contains all data from 2021 (consisting of df3 and df4), names not yet processed (cannot be disclosed).
3. Complete Data:
    `sr` (system report, merged from df2020 and df2021), names processed (can be disclosed).
    
    - Field Description:
    `student`: Name code
    `year`: Data source year, either 2020 or 2021
    `class_year`: Grade level, either 6 or 7
    `class_name`: Class identifier, either C, K, or T
    `book_planned`: Number of books planned to read
    `book_passed`: Actual number of books read
    `A+`, `A`, `B`: Scores obtained from reading books
    `planning`, `execution`, `knowledge`, `improvement`: Four quantitative scores based on reading performance
    `total_skills`: Composite score including the above quantitative scores and other performances (not included in this data)
    `honor_given`: Points awarded based on reading performance
    `final_score`: Reading assessment score (independent test, unrelated to the aforementioned reading performance)
    `study_year`: Academic record, L (only read in 2020), N (only read in 2021), B (read in both years)
    
## III. Data Processing Details

### Step One: Processing Data from 2020

    1. Import data from 2020 (two datasets) and merge them into one dataset.
    2. Remove unused columns, rename columns, and add a column to mark 2020.
    3. Handle null values, duplicate values, and eliminate invalid data.
    4. Initial observation: Examine distribution, correlation, visualization.

### Step Two: Processing Data from 2021
   
    5. Process data from 2021, repeating the first step process.
    
### Step Three: Processing Data from Both Years

    6. Change names to codes, and categorize: Only read in 2020 (Left), only read in 2021 (New), read in both years (Both).
    7. Merge all data.
    8. Save.

### Step Four: Visualization and Analysis

    9. Second observation: Examine distribution, correlation, visualization.

* Additional Information: The original data contains personal information, so only the code is provided for reference. The final presented data and analysis are results with **personal information removed** and **data adjusted**.