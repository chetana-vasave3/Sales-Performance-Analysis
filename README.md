
# Sales Performance Analysis



## Index

 - Objective 
 - Data Understanding
 - Dataset Description
 - Exploratory Data Analysis
 - Data Visualization
 - Conclusion




## Objective

Analyze the dataset to assess the performance of different primary producers, sales teams, or account managers in the years of 2017,2018 and 2019. Identify top performers, evaluate their strategies, and derive insights to improve overall sales performance.Visualize the data to uncover insights and make informed business decisions based on historical sales performance.

## Data Understanding
First of all we have to understand the data provided by the client in order to make tha data ready for analysis.
Domain: The dataset appears to be related to sales or business development, specifically in the insurance.  It captures information about sales opportunities, their stages, accounts, niche affiliations, expected decision dates, annual revenue, account IDs, and office locations.

 In first step we have consolidate all the data that client have provided us in 3 different table format. you can refer the csv file provided in this Repository as  Sales Performance analysis.csv and Cleaned_consolidated_Tables.csv

 
##  Dataset Description
- Date: Represents the date when a particular event or interaction occurred, such as a meeting or review.

- Primary Producer: Refers to the primary producer or salesperson responsible for handling the opportunity.

- Stage Name: Describes the stage or status of the sales process for each opportunity, such as "1-Met Client, Data Gather, Insurer Market" or "2-Client Presentation-Await Feedback."

- Account Name: Specifies the name of the account or customer being targeted for the opportunity, such as "West Point Construction Ltd" or "Newmor Group Limited."

- Opportunity Name: Identifies the name or identifier assigned to a specific sales opportunity, such as "Meeting 06/03/2019" or "2019 Review."

- Niche Affiliations: Represents the specific affiliations or industry segments associated with the opportunity, such as "Construction," "Transportation," or "Commercial - All Other."

- Expected Decision Date: Indicates the anticipated date when a decision is expected to be made regarding the opportunity.

- Annual Revenue: Represents the annual revenue associated with the account or customer, providing a measure of their financial scale.

- Acct ID: Provides an identifier for each account.

- Primary Office: Indicates the primary office associated with the account.

- Office: Specifies the office location related to the opportunity.


## Exploratory Data Analysis

 After merging all the tables our very next step was to do data cleaning process so that we can get some accurate insights from that cleaned data.
 so we checked for duplicate values, Missing values and Outliers in the dataset . We removes all the duplicate values from the daatset and filled missing values by using some statistical methods like mean, median and mode.

 Now from data understanding we could able to get that the provided data is related to datetime like the sales in the year 2017, 2018 and 2019..so our very next step was to convert the data type of the date column to Datatime and extract month ,year and day from the date column. 

 Now we could able to see year wise annual revenue and avarage annual revenue.


### Annual Revenue by Year
![Annual Revenue by Year](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/Annual%20revenue.png?raw=true)

- So, here we can get insight like year 2017 has maximum average annual Revenue and year 2019 has maximum annual Revenue

- we can group the accounts by their primary producer and analyze which producer brings in the most revenue or which producer has the most accounts.

![Annual Revenue by primary producer](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/Annual%20revenue%20by%20primary%20producer.png?raw=true)


### Count of Account Names by primary producers
![Account names by primary producers](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/count%20of%20account%20name%20by%20primary%20producer.png?raw=true)

- from above we can say Producer 3 has most no. of counts of Acoounts and Producer 5 brings the most revenue.

The difference between the expected decision year and the year of account generated can give insights into sales cycle of the business. if the difference is relatively short, it may suggest that the sales process is efficient and leads are being converted quickly.


#### Avg_time_taken_to_take_decisions by primary producers
![Avg_time_taken_to_take_decisions by primary producers](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/avarage_time_taken_to%20take%20decision.png?raw=true)


### Distribution_of_Annual_revenue

![Distribution_of_Annual_revenue](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/distribution%20of%20revenue.png?raw=true)



Now, we can perform Annova test between primary producer and annual revenue to test if there is significant difference in the mean annual revenue generated across different primary producers. this can help to identify which primary producers are most profitable.

### Most Profitable primary producer

![Most Profitable primary producer](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/Top%20Producer.png?raw=true)



### Top 5 Profitable Account Names

![Top 5 Profitable Account Names](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/top5%20account%20names.png?raw=true)


### Top 5 Profitable Account Names by year

![Top 5 Profitable Account Names](https://github.com/chetana-vasave3/Sales-Performance-Analysis/blob/main/Screenshots/top5%20account%20names%20by%20year.png?raw=true)


##Conclusion

- Year 2017 Has Maximum Avg Annual Revenue
- Year 2019 Has Maximum Annual Revenue.
- Producer 5 Has Maximum sum of annual revenue
- Producer 3 has maximum Account Names
- Producer 4 can take quick Decisions and it may suggest that the sales process is efficient and leads are being converted quickly.
- Producer1 is most profitable in the year of 2019,2017 and 2018 because it has max avg revenue
- We could able to find Top 5 most profitable Accounts in this years.
