# Unicorn-Companies

### Dashboard Link : https://app.powerbi.com/groups/me/reports/97b98dd3-18db-440c-ab15-be0c86e3b9ac/ReportSection799ca1071d968077feea

## Problem Statement

We are interested in konowing about the valuations and fundings of unicorn companie. Also a detailed analysis of industries getting funding is to be done. Several other insights to be drawn in order to know the country and city with good number of unicorns. Also we are interested in knowing the time required by companies belonging to different industries in becoming a unicorn company.

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
- Step 5 : Also since all investors for a given company were given in one row (each investor name separated by a comma), so first of all column named "investors" was split at each occurance of delimiter in power query editor & then unpivot columns feature was used to bring all of them in one column.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Blank records created due to presence of two consecutive delimiters were filtered out using text filter in power query editor. 
- Step 8 : Columns named "funding" and "valuation" were textual columns, they were converted into numberical columns by using various transformation options. 
- Step 9 : On first page of report a slicer was added for selecting particular company name,five cards were added and a table was added to show the names of the investors & a map visual was also added to show the names of the city.
- Step 10 : Under the insert tab using image option in report view an image was added on the first page.
- Step 11: On the second page following visuals were used to convey insights,
 A bar chart showing top 5 countries with highest number of unicorns.
 A column chart showing top 5 unicorns by valuation.
 
      (a) A line chart showing number of unicorns by year.

      (b) A multi row card was used to show top 3 industries by valuation.

      (c) A multi row card was used to show top 3 industries by funding
