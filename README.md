# An Analysis Report of Kickstarter Campaigns in Relation to Launch Dates and Funding Goals

### Kickstarter Campaign Analysis Overview

This analysis report aims to help visualize comparative theater campaigns by launch dates in monthly periods and set goals on what trended successful, failed, and canceled campaigns.  In this analysis, there will be diagrams of two primary methods of representing data:

1. Outcomes based on launch date.
1. Outcomes based on goals.

This is in order to give a clear indication of measured success by correlating not only goals set but what timeframes to best launch a campaign.

### Analysis and Challenges

#### Analysis

In this analysis, we will review the first dataset of outcomes based on launch date to give an idea of how kickstarter theater campaigns fared by months.  In this dataset, the sample amount was a grand total of 1,369 unique campaigns collected worldwide between the years 2009 to 2017.  The formula used to determine the years in our filter is displayed in Chart 1.

		**Chart 1**: "Excel Formula YEAR()"
				=YEAR(@S:S)

The majority of these campaigns did come from the US at 900, with the next largest from Great Britain at 353.  Regardless, they both averaged relatively similarly and had the biggest impact on the given data displayed in Chart 2.

		**Chart 2**: "Theater Ouctomes Based on Launch Date"
![Theater_Outcomes_vs_Launch](resources/Theater_Outcomes_vs_Launch.png)

In Chart 2, we can see the highest amount of successful campaigns launched in the summer months starting in May and progressively tapering by September.  It is noted that "Fever" launched in June and with further analysis, we have to take a look at another dataset of outcomes based on goals to see if there were any identifiable contributing factors on what otherwise is a great time period to launch a campaign.  In order to get the data needed another formula was required to count the number of successful, failed, and canceled plays displayed in the following Chart 3.

		**Chart 3**: "Excel Formula COUNTIFS()"
			Number Successful - Goal Less Than 1000
				=COUNTIFS(Kickstarter!D:D,"<=1000",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays")
			Number Failed - Goal Less Than 1000
				=COUNTIFS(Kickstarter!D:D,"<=1000",Kickstarter!F:F,"failed",Kickstarter!R:R,"plays")
			Number Canceled - Goal Less Than 1000
				=COUNTIFS(Kickstarter!D:D,"<=1000",Kickstarter!F:F,"canceled",Kickstarter!R:R,"plays")

A range of goals was created that started with 1,000 or less, and increased by increments of 5,000 until we came to 50,000 or more.  The counts were collected per range and then percentages were assigned to give a clearer picture of successful campaign goal ranges displayed in Chart 4.

		**Chart 4**: "Ouctomes Based on Goals"
![Outcomes_vs_Goals](resources/Outcomes_vs_Goals.png)

Chart 4 gives a very clear indicator that campaigns with goals of 5,000 or less were the most successful, and going beyond that especially 15,000 proved to be unfavorable.  However, there is an anomaly in the goal range of 35,000 to 40,000 with a decent measure of success.  The sample amount collected in that range was 6, compared to a sample collection of 785 in the Less than 1,000 to 5,000 range.  With the very small amount of samples in the higher range, it is advisable to err on the side of it being an outlier and not a clear indicator of success.

# !!!Need to complete in the morning | ~~Also Pictures in this README~~!!!

#### Challenges

### Results

## Outcomes based on launch date chart.

#### Conclusion One
#### Conclusion Two

#### *Figure 1*

## Outcomes based on goals chart.

#### Conclusion

#### *Figure 2*

## Limitations of the dataset
### Recommended tables or graphs

