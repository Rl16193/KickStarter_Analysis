# KickStarter_Analysis
Analyze data for Kickstarter campaigns across the globe and present Louise with information on trends 
## Overview
>Louise’s play Fever came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals.

Along with any additional trends we can highlight which would ease the decision making process.
## Analysis and Challenges
### Step by Step Analysis
Step 1: Initial look at the data presents us with an unreadable column Deadline and Launched_At. Use the formula shown to convert Unix timestamp to Date Format

![Date Conversion Formula](https://user-images.githubusercontent.com/100053788/158075345-65af4cb3-b4ba-4d1d-b6c0-f413301b9299.PNG)

Step 2: Extract the year the kickstarter was launched using YEAR() Function.

Step 3: Using Text to column separate Categories to Parent and Sub Category.

Step 4: Create Pivot table to obtaining a better understanding of outcomes vs launch dates. Group the Date row to show Months

![image](https://user-images.githubusercontent.com/100053788/158075577-e922941e-d51b-46f0-951a-044c61f04c69.png)

Step 5: Create another sheet and even distribute the goals observed. Increments can be selected on User assumption

![image](https://user-images.githubusercontent.com/100053788/158075620-d3f3c7b7-9716-4e3a-b275-7d37c0eafc20.png)

Step 6: Use COUNTIFS() function as shown to count the outcomes for each goal range.

![image](https://user-images.githubusercontent.com/100053788/158075647-eb30d7ff-29d5-4e72-82e9-4e3b95c2694d.png)

Step 7: Plot the Charts for Outcomes Vs Goals and Theather Outcomes by Launch Date
### Challenge Encountered
Grouping of data in the pivot table was difficult to do. Watching the video helped.

## Results
### Theater Outcomes vs Launch
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/100053788/158075817-aab174d4-cf30-4518-844c-783ee6a723a9.png)
1. The best tine to launch a Campaign is during the Months of May and June, **the best result is observed in May**, with the highest number of succesful campaigns for Theater.
2. Toward the end of the year (Novemeber and December) we observe a drop in the number of successful campaigns. The probablity of a Theater Kickstarter being successful is very low. **It is advisable to not launch a campaign during these months**. 

### Outcomes vs Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/100053788/158076016-7fad3197-c25a-415d-85e6-503c0c7c1119.png)
1. We observe a drop in successful kickstarters as the goal increases **(highest is for goal 0 to 1000)**. This trend sees a change between goal - 30000 to 45000 where there is an increase in the success rate of kickstarters. After this the downward trend resumes.

### Limitations
1. We need to sample the data more accurately to obtain better results. Removing outliers would help obtain better visual representation of the data.

### Recommendation
1. We can plot average donation Average donation with categories to better understand which category attracts more money.
2. We can plot average backers over categories to better understand which category appeals to a larger audience.
3. We can plot average backers and donation over months to see confirm the findings from Theater Oucome vs Launch Date Graph
