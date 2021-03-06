# kickstarter-analysis
# Kickstarting with Excel by David Aduaka 
## Overview of Project
Louise is a playwright who is looking to start a crowdfunding campaign to fund her play, Fever. She has a budget of over $10,000 and is seeking advice about how to successfully set up and execute her campaign. She came close to reaching her fundraising goal, and is now seeking advice about how different campaigns performed in relation to their launch date and fundraising goals.

To do this, I analyzed data from various Kickstarter campaigns to determine if there are any trends in start times, fundraising goals, or other factors that can be implemented in Louise’s project.

### Purpose 
The purpose of this analysis is to determine if there are any trends in start times, fundraising goals, or other factors that can be implemented in Louise’s project.

## Analysis and Challenges 
### Analysis of Outcomes Based on Launch Date

Using the Kickstarter data, I added a new column called Years, and converted the Date Created Conversion column to display the years. From this I filtered the date data to span from 2009 to 2017. I then created a pivot table, filtered by Parent Category theater, and counted the different outcomes for each month. I then created a pivot chart from this table, shown below.

![image](https://user-images.githubusercontent.com/70069730/148710195-f8ef7e42-ec0c-48d6-859b-2c76428c8244.png)

### Analysis of Outcomes Based on Goals

Using the Kickstarter data, I created a new graph that displays Outcomes based on each Plays' goal amount. I established bin sizes of approximately 5,000, and used the countifs function to show the number and percentage of each type of outcome. This graph is shown below.

![image](https://user-images.githubusercontent.com/70069730/148710361-519d9f75-c13e-4e34-813e-086e55c33547.png)

### Challenges and Difficulties Encountered

The data required formatting that added to the analysis time. First, the Unix timestamp format in the Deadline and Launched_at columns added a layer of difficulty to the analysis and had to be converted to a readable date. Second, the blurb information had typos and unusual characters, which can be shown in the Edinburgh Research tab of the workbook. If someone were performing an analysis based on information in the blurbs, he or she may have a hard time reading it.

## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date? First, Theater Kickstarter campaigns that launched in May were significantly more successful than campaigns launched in other months. Second, campaigns launched in October were almost equally as likely to succeed as to fail. From these two conclusions, I would recommend to Louise that her campaign would fare best if launched in May, and at latest, be launched in September.

- What can you conclude about the Outcomes based on Goals? The table in the Outcomes Based on Goals tab shows that most of the play campaigns (approximately 92%) had goals of $14,999 or less, and that 95% of all successful play outcomes fell in that same Goal range. I would conclude that this is the target goal range Louise should have aimed for.

- What are some limitations of this dataset? One limitation of the data is how current it is. The data has results only through 2017 and we are performing this analysis in 2021. Additional current data would be helpful in determining trends and factors. Another limitation are the text. As mentioned before, the blurbs contain typos and unusual characters. Finally, there is no definition of what the staff_pick and spotlight columns refer too. If they are in relation to popularity or if they were promoted more frequently, this could have been used to advise Louise on planning her campaign.

- What are some other possible tables and/or graphs that we could create? One additional graph would be a histogram of the Outcomes Based on Goals, rather than a line chart. This would show her how the bins looked and where the mean of the data lay. Another graph would be re-filtering the PivotChart and Pivot tables by subcategory “plays”. This would have drilled down directly to the plays subcategory. Finally, I would create a table of successful US plays with goals of $14,999 or less that opened in May, using VLookup functions to pull names and blurbs. Then, through analyses of these blurbs, I would identify the genres of these plays to determine what people found popular and funded. I could present this to Louise to see how well received her campaign would be.




