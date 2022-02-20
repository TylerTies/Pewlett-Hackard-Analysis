# Pewlett Hackard Analysis

## Project Overview
Further analysis was requested to determine if there was an opportunity for a mentorship to help manage the number of upcoming retirements.  The first step was to find the number of retiring employees per title and the second step was to identify employees who would be eligible for the mentorship program.

## Resources
- Data source: departments.csv, dept_emp.csv, employees.csv, titles.csv
- Software: pgAdmin4 6.1, PostgreSQL 14.1, Visual Studio Code 1.64.2

## Results
This analysis looked at both the number of employees as well of the makeup of their roles and departments to determine what impact the "silver tsunami" in the coming years.

- **Size:** The first major data point that jumps out from the analysis is the sheer size of the potential retirees from the three years in the analysis. There were 72,458 total employees in this dataset.  That's a massive undertaking in hiring alone.

![Retiring Titles Summary](/data/retiring_titles_count.png)

- **Senior Positions:** The next point that was quickly apparent was the highly skilled positions in the retirement pool. The Senior Engineer position alone could potentially lose nearly 26k due to retirement. This could be filled with lower level employeees already in the company through promotions but may need to be heavily recruited if the current employee pool doesn't have enough candidates.

- **Other Positions:** There are also nearly 10k Engineers that could potentially retire which would further reduce this labor pool needed to replace the departing senior engineers.

- **Mentorship Eligibility:** The mentorship eligible pool was only 1,549.  This could create issues if these employees are expected to mentor enough people to backfill the retirees.  Some departments may be impacted more severly than others and having few mentors might cause issues.

## Summary
-   How many roles will need to be filled as the "silver tsunami" begins to make an impact? Based on the qualifications, the three years of retirement eligible employees amount to potentially losing 72,458 employees.

-   Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?  With only 1,549 employees determined eligible in our analysis this could be a real problem.  These employees would be expected to mentor a high number of new employees and could be stretched thin depending on the departments in which they reside.

I wanted to further investigate the distribution among the departments of each population.  Using the existing tables from the analysis, I created the following queries to pull the distribution for each population.

![Queries](/data/query_screenshot.png)

The queries gave me the counts by department for each population.  I then put this into excel to format a table and compare the percent of total across the departments.

![Department Breakout](/data/department_breakout.png)

This confirmed that the mentor breakout across departments is fairly close to the breakout seen across the population of potential retirees.  The mentors appear to be located in the right departments.  My concern is the lack of mentors overall.  From the data above, it would appear the average mentor would need to cover over 45 new employees each.  More mentors may be needed depending on the experience and timing of new employees and whether these employees come from external to the company or are internal hires.