## **VILLENA_PA4 2ECE-B ECE 2112**

## Intended Learning Outcomes

At the end of this laboratory activity, the student should be able to:

1. filter tabular data using several categorical and numerical conditions;

2. construct focused DataFrames by selecting relevant features;

3. summarize the relationship between categorical features and a numerical variable; and

4. communicate a data comparison using clear and correctly labeled plots.

## Instructions

Use the same ECE Board Exam 2 dataset supplied for Experiment 4. Work in a Jupyter Notebook
using Pandas and a Python plotting library used in class. Use the dataset’s existing column labels,
including Name, Gender, Track, Hometown, Math, GEAS, Electronics, and Average.

• Derive all tables and plot values from the dataset. Do not manually type rows, category means, or
plotted values.

• When applying more than one condition, make every condition explicit in the filtering expression.

• Keep the original DataFrame unchanged.

• Every graph must have a title, axis labels, readable category labels, and a consistent scale appropriate
to the data.

 

## A. VISAYAS COMMUNICATION DATAFRAME

The task in this problem is to filter Visayas students under the Communication track and keep the required columns.

The following functions and methods were used in this problem:

• **mean(axis=1)**	—— calculates the average across the subject columns for each student

• **Boolean filtering**	—— selects rows based on True or False conditions (mostly incorporated into df[])

• **==**	—— checks if a column matches a specific value

• **&** —— combines conditions where both must be true

• **df[[...]]** —— selects multiple columns

• **len()** —— counts the number of rows


 

**Explanation of method used:**

The hometown and track conditions are combined to filter the dataset. The required columns are then selected from the filtered results.

 

## B. VISAYAS FEMALE DATAFRAME

The task is to filter female students from Visayas and display those with an Average of 60 or higher.

The following functions and methods were used in this problem:

• **display()** —— shows the DataFrame as a table

• **print()** —— outputs text or values

• **==** —— checks the hometown and gender conditions

• **&** —— requires both conditions to be true

• **df[[...]]** —— selects the required columns

• **>=** —— checks if the Average meets the minimum value

• **VisFemale[...]** —— applies another filter without changing the original DataFrame


 

**Explanation of method used:**

The first filter creates **VisFemale** using hometown and gender. A second condition is then applied to display only students with an Average of at least 60.

 

## C. CATEGORY-AVERAGE VISUALIZATION

The task is to calculate the mean Average for each Track, Gender, and Hometown, then compare them using bar charts.

The following functions and methods were used in this problem:

• **groupby()** —— groups the data according to a categorical column

• **.mean()** —— calculates the mean Average for each group

• **axes[]** —— accesses each individual chart so it can be customized

• **print()** —— displays the calculated results or interpretation statements

• **.plot(kind="bar")** —— creates bar charts from the calculated results

• **.idxmax()** —— identifies the category with the highest mean

• **plt.subplots()** —— places the three charts in one figure

• **set_title() , set_xlabel() , set_ylabel()** —— adds titles and axis labels


 

**Explanation of method used:**

The data is grouped by each categorical feature, then the mean **Average** is calculated. These results are used directly for the summary tables and bar charts, while **.idxmax()** identifies the highest observed mean.

 

 

Thank you for Reading!

To see the main python program for Programming Assignment 1, click this link https://github.com/josegabrielvillenaeng-coder/Villena_ECE2112_PA4/blob/main/VILLENA_2ECEB_PA4.ipynb
