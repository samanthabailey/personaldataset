# personaldataset
# Motivation 
### My motivation behind selecting this data set was based purely on the fact that I am double majoring in Criminal Justice so I wanted to do something pertaianing to that. Additionally, whenever I hear people talk about serial killers, they tend to think of the United States first hand. Thus, I liked this data set because it contained data for serial killers that was obtained world wide rather than just the United States. Furthermore, I mainly wanted to look at the numbers and compare them via country and also see if there was any correlation between how long a killer was active and their victim count. 

# Data Process
### My process for obtaining the source was through Kaggle. The data set was scraped off of Wikipedia's page of Serial Killers. My first step in the cleaning process was to make sure everything was in correct format. I changed some of the date ranges to fit the "year to year" format. Next, I added a column that calculated the difference between the last and first years active so I could have a column with a simple number that would be easier to work with for this process and the questions I needed to answer. I then decided to cut the original line 26 due to lack of record of time period. Next, I went into all cells that had multiple countries and only kept the countries where the crimes were committed and were confirmed, not "alleged". Finally, I deleted the notes column because the notes were not relevant to exploring this data set. 

# Visualizations
### I made two visualizations for this data set. Both histograms but both look at the distribution of two different variables amongst the data set.
![image](https://user-images.githubusercontent.com/91634200/144734415-284dbc72-50a3-449d-b157-05f68c6125b1.png)
This histogram looks at how the number of proven victims is distributed.

![image](https://user-images.githubusercontent.com/91634200/144734432-a894a21b-fb41-49ce-996d-8f9b0309c3b3.png)
This histogram looks at the distribution of number of years active.

# Analysis
### In my R markdown file I mainly analyzed the relationship with years active and proven victims. I began by looking at Tukey's five number summary for both variables. The years active variable has a minimum of 1 year and maximum of 36 years. The median was 7 years while the mean was 10.12. 
### For the proven victims variable, the minimum was 32 with a maximum of 138. The median was 48 with an average of 53. Then I looked at the value of correlation between years active and proven victims and it was only .03 which indicated not a very strong correlation between the number of victims and how many years a killer operated. 
### Finally, I did a little bit of analysis with logistic regression with Country as the "response variable". Based off of this I got an equation that would look like the following: 
Country= -0.037914358(years active) + 0.000672292(proven victims)+ 2.706309726  
### In Excel, I also created pivot tables to analyze specific variables and their relationship. The first was a comparison of highest victim counts between countries. United States came first with a sum of 212 proven victims and Egypt was last with 32 proven victims. Then, I created a pivot table that looked at each individual and how their years active compared to their victim count. The person with the highest victim count was only active for 7 years. 
