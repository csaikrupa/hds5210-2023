# Feedback on your final

**Final Score: 52/60**

The grading rubric for the final can be found in GitHub: https://github.com/paulboal/hds5210-2023/blob/main/final/final-instructions.pdf

**Functional Requirements**
* 5 points - Uses data from at least two different sources: local file, internet, web service, relational database, AWS S3, etc; and formats: CSV, JSON, database, XML, Excel, etc
* 5 points - Data from multiple sources has to be joined together at least twice
* 5 points - Data is aggregated or pivoted at least twice during the program
* 5 points - Some kind of field-level transformation is performed at least 5 times
* 5 points - The program creates 3 or more data visualizations 
* 5 points - The program serves a theoretical purpose described in documentation, that could potentially do something in healthcare or another industry of interest

**Modularity / Style**
* 15 points - The code is broken up into various functions or classes to make testing and reuse easier

**Documentation and Professionalism**
* 15 points - All functions are documented and notebook cells include annotations and explanations.

**(-1) Variable names like `dd_df1` or `dd_df2` aren't helpful to the reader.  You should use variable names that better explain what the data is and why we're interested.**

**(-1) When you create functions, you should always include docstrings; and should include doctests when appropriate.**

**(-1) Some of your "explanation" comments merely describe what you're doing rather than explaining WHY you're doing it and what will come next.  There's a section for dd_df1 where you're convering several columns to numeric.  You've copied/pasted the code and documentation multiple times.  You could have done that far more efficiently with a loop"**
```python
# Here we convert these columns to a numeric data type to be sure we can compute 
# statistics on them.  I plan to compute BMI using these values and then look
# at some averages across different regions and years.
for col in ['AGE','HEIGHT','WEIGHT']:
    dd_df1 = convert_column_to_numeric(dd_df1, col)
```

**You should not have named a variable `json`. It doesn't describe what data you'll find there and it is commonly used python library**


**(-5) You didn't merge or join the data anywhere**

**I think you did a fine job on this final.  There were several areas where you could have been more efficient and you failed to meet the merge/join requirment, but what you did was solid coding.**