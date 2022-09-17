# Unicorn-Companies

### Dashboard Link : https://app.powerbi.com/groups/me/reports/97b98dd3-18db-440c-ab15-be0c86e3b9ac/ReportSection799ca1071d968077feea

## Problem Statement

This dashboard conveys insights related to unicorn companies.

There are three pages in the report, 

First page conveys details of a given unicorn company when selected using a slicer, 

Second page gives a description of top 5 countries with highest number of unicorns, top 5 unicorns by valuation, top 3 industries by valuation, top 3 industries by funding & number of unicorns by year.

Third page gives the detail of unicorns in which a given investor has invested.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "City" in which some values were null values.
- Step 5 : For calculating average delay time, null values were not taken into account as only less than 1% values are null in this column(i.e column named "Arrival Delay") 
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since the data contains various ratings, thus in order to represent ratings, a new visual was added using the three ellipses in the visualizations pane in report view. 
- Step 8 : Visual filters (Slicers) were added for four fields named "Class", "Customer Type", "Gate Location" & "Type of travel".
- Step 9 : Two card visuals were added to the canvas, one representing average departure delay in minutes & other representing average arrival delay in minutes.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.
- Step 10 : A bar chart was also added to the report design area representing the number of satisfied & neutral/unsatisfied customers. While creating this visual, field named "Gender" was also added to the Legends bucket, thus number of customers are also seggregated according the gender. 
