# Kickstarting with Excel

This project constitutes the Module 1 Challenge for the Data Analytics and Visualization Boot Camp.

## Overview of Project

### Purpose

An aspiring playwright, Louise, has written a play and is wondering if her estimated budget of over $10000 is too ambitious. This project helps her determine if her crowdfunding goal for her play will be conducive to success based on previous crowdfunding campaign data by utilizing Excel tools such as Pivot tables and descriptive statistics. 

## Analysis and Challenges

Louise has data in the form of an Excel spreadsheet with Kickstarter campaign funding data. See [a screenshot of the image of the dataset](https://github.com/josephrodini/kickstarter-analysis/blob/main/dataset.PNG). Two main analyses were performed on this dataset. The first was an analysis of outcomes based on launch date, and the second analysis was outcomes based on goals. 

### Analysis of Outcomes Based on Launch Date

First, to help Louise determine if there are any particular months of the year during which crowdfunding campaigns are more successful, an analysis of outcomes based on launch date was performed. A “Years” column was created based on the “Date Created Conversion” column in the Kickstarter spreadsheet. A pivot table was then created in a worksheet called “Theater Outcomes by Launch Date”. Filters were created for “Parent Category” and “Years." The “Parent Category” was filtered on “theater." The row labels were changed to display the months of the year, and the campaign outcomes were sorted in descending order. Finally, to help visualize the data in the table, a line chart was created showing the number of successful, failed, and canceled projects by month. A “Years” column is created based on the “Date Created Conversion” column in the Kickstarter spreadsheet. A pivot table was created in a worksheet titled “Theater Outcomes by Launch Date” with filters on the “Parent Category” and “Years” data columns. The “Parent Category” was filtered on “theater.” The row labels were changed to display the months of the year, and the campaign outcomes are sorted in descending order. Finally, to help visualize the data in the pivot table, a line chart was created showing the number of successful, failed, or canceled projects by month. See [Theater Outcomes vs. Launch line graph](https://github.com/josephrodini/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png).

### Analysis of Outcomes Based on Goals

Second, to help Louise determine what goal value crowdfunding campaigns prove most successful to fund, an analysis of analysis of outcomes based on goals was conducted. A spreadsheet was created called "Outcomes Based on Goals." The COUNTIFS() function was used to determine the number of successful, failed, and canceled campaigns in 12 ranges of goal budget values, from less than $1000 budget to over $50000 budget for the subcategory "plays." The sum of the successful, failed, and canceled plays was determined in a new data column. Using the total number figures, the percentages of successful, failed, and canceled projects were calculated and placed in new columns. Finally, to help visualize the data in the spreadsheet, A line chart entitled "Outcomes Based on Goal" was created with the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis. See [Outcomes Based on Goal](https://github.com/josephrodini/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png).

### Challenges and Difficulties Encountered

This dataset presented no major challenges or difficulties when analyses were performed on it. But if data had been missing from the dataset, such as information on the category of the production or the crowdfunding goal, analyses would have been harder to complete and conclusions harder to infer.  

## Results

### Outcomes Based on Launch Date

Based on the outcomes based on launch date pivot table and associated line graph, we can draw a few conclusions. The best time for success in a crowdfunding campaign seems to be the summer months, with May in particular being the month with the highest success rate. The number of canceled campaigns seems to be quite low in comparison to successful and failed campaigns, and more or less evenly dispersed across the months of the year, with the exception of October which had no canceled campaigns.

### Outcomes Based on Goals

Based on the outcomes based on goals analysis, we can learn several things. Louise's budget is in the range in which about 54% of campaigns are successful based on their budget goal. This is better than a 50/50 chance, however lower budgeted plays have even a higher success rate. In contrast, plays with budget goals of $25000 to $34999 are much more likely to fail. However, the sample of higher valued budget goal plays is quite small and therefore might be more unreliable. 

### Limitations

This dataset is quite comprehensive, with data from many countries across many categories of production. However, it has its limitations. For example, the data was all collected before the COVID pandemic, which might have significantly impacted the success rate of crowdfunding campaigns. More recent data would be beneficial. Also, this dataset could have contained several other measures that would have been helpful, such as subdivision of the goal budget for paying actors, set design, etc. Finally, it is unclear how the US dollar equivalencies were calculated for campaigns funded in other currencies. The data from other countries might be skewed as a result.

### Other Tables and Graphs 

There are many additional analyses that could be performed on this dataset. I wonder how the length of the crowdfunding campaign affects its likelihood of success. To answer this question, a table much like the one created in the outcomes based on goals could be created entitled "outcomes based on campaign length," with different ranges of campaign length and their corresponding success and failure rates. We could also do analysis of play campaign success rate by country, using a bar chart to graph in which countries play campaigns are most likely to reach their budget goals.
