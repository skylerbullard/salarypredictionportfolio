# salarypredictionportfolio

## salary prediction project

This portfolio project will help predict what potential salaries are for specific job types. An amount of data at our disposal carries information about job types in particular industries across the globe. Salary prediction will be aided by three mean-squared-error machine learning models.

The first jupyter notebook will further the definition, examination, exploration, and overall discover of job description data.

## step 1) examine the data, features

jobId - unique identifier consisting of letters and numbers

companyId - unique identifier consisting of letters and numbers

jobType - categorical value, the job's hierarchy placement in a company

degree - categorical value, type of educational diploma

major - categorical value, description or focus of degree

industry - categorical value, description of professional sector in society

yearsExperience - quantitative value, amount of time person spent in role

milesFromMetropolis - quantitative value, distance from company works for

## step 2) find potential outliers

I used the Interquartile Range (IQR) rule to locate potential outliers that fall out of upper and lower bounds. The zero salary entries are not volunteer positions. These are instances of missing/corrupt data. Zero salary jobs will be removed from the dataset. The high-salary potential outliers appear to be legitimate. C-level executives are in high salaried industries. The junior roles are in the same high salaried industries (oil, finance). These potential outliers will remain. 

## note: preparing for modeling - the target attribute is salary (a number), which is not a category so classification may not be the best appproach; rather a regression model may be better.
