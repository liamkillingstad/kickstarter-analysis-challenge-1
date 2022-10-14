# Kickstarting with Excel

## Overview of Project
The project stipulates that we analyze the kickstarter dataset in order to provide insights about the potential kickstarter campaign for Lousie's play *Fever*. The dataset provides a vast array of information about different kickstarters, their relative success, metrics around funding, and additional information. Our aim is to segment the information to look specifically at how kickstarter campaigns for plays have fared under various circumstances according to the dataset. 
### Purpose
The task at hand is to filter the kickstarter data provided to specifically encapsulate the historic kickstarter outcomes for plays based on their launch dates and fundraising goals. By examining the existing data, we hoped to be able to draw certain insights about fundraising targets and timing that would help ensure the successful launch of the *Fever* kickstarter campaign. 
## Analysis and Challenges
In order to manipulate the data, we creatd two seperate pivot tables and associated charts that showed how kickstarters - specific to plays - fared during a given month OR given a certain range of funding goals. Below, I have provided an analysis of the impact of these two factors on the existing kickstarter dataset. 
### Analysis of Outcomes Based on Launch Date
The analysis based on launch dates was conducted by creating a pivot table to examine specifc months in which theater campaigns were conducted and to chart the relative frequncy of those outcomes over time. In the image below, the chart mentioend can be referenced. 
According to the data, there are similar observable patterns that occur between failed and successful kickstarter campaigns in any given month. More specifically, the data's directional moves (increase or decrease) were the same or similar for failed and succesful campaigns in all months except from November to December where the number of succesful campaigns decreased and the number of failed campaigns increased. 
In the image included below, we can see that the failed kickstarter campaign data tends to follow a similar shape to the succesful campaigns over time, just at a lower maginitude.
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/115036844/195756099-cb5a4bf5-364c-4261-889f-ba1f10450646.png)
There seems to be a slighly positive correlation between the success and failure of a campaign in any given month (i.e. if the number of succesful kickstarters increased from January to February it is likely that the number of failed kickstarters failed as well). Additionally, The earlier and later months seem to demonstrate the least amount of overall activity relative to the middle (summer) months. 
Data regarding the canceled campaigns was relatively flat indicating that there were not strong seasonal effects determining whether or not a campaign would be canceled. 
All references to the data can be found in the excel sheet linked below
[Kickstarter_Challenge.xlsx](https://github.com/liamkillingstad/kickstarter-analysis-challenge-1/files/9782252/Kickstarter_Challenge.xlsx)
### Analysis of Outcomes Based on Goals
The outcomes based on goals analysis was conducted by utilizing excel's *COUNTIFS* functionality to determine how many succesful, failed, and canceled campaigns were conducted within specified "raise targts". The raise targets were denoted in $5,000 increments from $0 through figures greater than $50,000. 
In order to manioulate the data, we were required to utilzie multiple if statements to classify data from the main sheet to satisfy the "play" category, the raise amount, and the level of completion (succesful, failed, canceled).
We then calculated the percentage associated with each kickstarter campaign goal range across succesful, failed, and canceled campaigns. The output can be seen in the image below. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/115036844/195756170-f8cde05b-a967-49fa-8369-44f837ed1247.PNG)

According to the data, there were no theater kickstarter campaings cancelled for any given fundraising target. Additionally, it appears as though the success rate of a given campaign steadily declines from a success % standpoints from the the less than $1,000 band until approximately the $25,0000 to $29,999 band. The inverse is true for the % of failed campaigns. 
The inverse symmetry of the graphs can be seen in the image provided below. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/115036844/195756170-f8cde05b-a967-49fa-8369-44f837ed1247.PNG)
All references to the data can be found in the excel sheet linked below
[Kickstarter_Challenge.xlsx](https://github.com/liamkillingstad/kickstarter-analysis-challenge-1/files/9782252/Kickstarter_Challenge.xlsx)
### Challenges and Difficulties Encountered
While there were no challenges in putting together the analysis, there could have been some difficulties when calculating the various conditionals within the "Outcomes Based on Goals" Analysis. 
## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
First, the shape and direction of the data for both failed and succesful campaigns are somewhat correlated while they are different in magnitude. It can be inferred that, given the positive correlation, that an increase in the number of succesful campaigns in a given month would likely also lead to an increase in the number of failed campaigns in that same month.
Second, there seem to be certain seasonal facotrs at play in the data. The number of failed and succesful campaigns seem be at or around their lowest during the first and final three months of the year. This would insinuate that duruing colder months (assuming non hemisperic geography) it is more difficult to succesfully execute a campaign.
### What can you conclude about the Outcomes based on Goals?
According to the data provided, there is a perfect inverse relationship between the % of succesful campaigns versus the % of failed campaigns for any given fundraising band. This is due to the fact that, in the dataset, there were no canceled campaigns for any of the given fundraising bands. 
From a data distribution stnadpoint, there was a steady decline in the % of succesful campaigns from $0 < $5000 to $25000 to $29999 fundraising bands. This indicates that smaller campaigns are incrementally more successful up until a certain inflection point. That inflection point appeaars to be approximately $30000 at which point we see a steady increase up to a local maximum of about 67% success at $45000. This all indicates that, in order to raise a succesful kickstarter for a theater performance, it is important to operate either with a very lean (low total fundraising goal) budget or a moderate to high budget (around $30000 to $45000). 
### What are some limitations of this dataset?
There are various limitations to the dataset. One important limitation to note can be reflected in our manipulation related to the "Outcomes Based on Goals" analysis. The sameple sine (*n*) of the data for each individual fundraising band becomes incrementally small and therefore less statistically significant. By manipulating the data the way that we did, we have reduced the reliability of data outcomes due to sample size. 
Additionally, The data provides information about kickstarters from 2009 through 2017. There are a multitude of exogenous factors (including but not limited to economic factors) that could be key drivers in why certain behaviors are occuring. Given the limitations of the dataset, we cannot be sure of the uniformity of exogenous variables in the fundraising environment. 
### What are some other possible tables and/or graphs that we could create?
An interesting additional analysis could be to see what the relationship is between the amount of money raised (as either an absolute value or the % of the total) and the total number of backers associated with the kickstarter. 
This could be useful in determinig whether or not a strategy for fundraising should be centered around reaching out to a large number of individuals for small checks or if it would be more advantageous to look at raising large lump sums of money from individuals.
