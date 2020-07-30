# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this project was to help Louise understand how different campaigns fared in relation to their launch dates and funding goals. Her play, *Fever* came close to its fundraising goal in a short amount of time, and she wants to see the outcomes of other campaigns. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The first step in helping Louise understand how the different campaigns fared was using the `Year()` function to isolate the Launch Date of each project. After this, I created a pivot table to filter the three outcomes (Successful, Failed, and Canceled) by the Parent Category. The dataset contained campaigns that were not theater plays, so it was important to filter the Parent Category to *theater*. From this pivot table, I was able to create a line chart that visualizes theater outcomes based on their launch date [Theater Outcomes Based on Launch Date](docs/Theater_Outcomes_vs_Launch.png) . 

### Analysis of Outcomes Based on Goals

The next part of this analysis was understanding how different campaigns fared in relation to their funding goals. In order to do this, I needed to visualize the percentage of successful, failed, and canceled plays over multiple dollar-amount ranges so the projects can be grouped based on their goal amount. Using the `Countifs()` function, I calculated the **Number Successful**, **Number Failed**, and **Number Canceled** in three columns. After this, I used the `Sum()` function to add the three outcomes in the **Total Projects** column, and divided each outcome by the total projects to get the percentage of each outcome. The enabled me to create a line chart to visualize the outcomes based on goals [Theater Outcomes Based on Funding Goal](docs/Outcomes_vs_Goals.png) .

### Challenges and Difficulties Encountered

One of the difficulties I encountered with this project was that the `Countifs()` function requires you to set criteria that is not linked to a cell. On my first attempt of analyzing the outcomes based on goals, my line chart did not look the same as the example chart in the module. After going through my work I realized I had misspelled “successful” in my formula, and it was returning an incorrect value because of that. 

## Results

Based on the Outcomes Based on Launch Date analysis, I can conclude that there are more successful theater kickstarter campaigns in the month of June than any other month. I can also conclude that the three months with the most successful campaigns happened during the summer season (May - July). Based on the Outcomes Based on Goals analysis, I can conclude that there was a higher percentage of failed campaigns when the funding goal was between $20,000 and $30,000. 
One of the limitations of this dataset was that there was no way to distinguish what genre of plays the campaigns were. It would be helpful if we could show how different plays fared if they were comedy, or musicals, or thrillers. Another graph that would’ve been helpful is if I showed the average donation relative to the funding goal. This might help explain why the percentage successful and percentage failed invert twice in the Outcomes Based on Goals analysis. 
