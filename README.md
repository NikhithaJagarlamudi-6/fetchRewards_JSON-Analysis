# fetchRewards_JSON-Analysis
## Overview
This project demonstrates how to reason data, transform unstructured JSON data into a structured relational model, generate meaningful queries for business insights, and identify data quality issues. Additionally, it includes a communication draft for stakeholders.
## Objective/ Task
1.	Review unstructured JSON data and diagram a new structured relational data model
2.	Generate a query that answers a predetermined business question
3.	Generate a query to capture data quality issues against the new structured relational data model
4.	Write a short email or Slack message to the business stakeholder
________________________________________

## Reviewing Unstructured JSON Data
### Files Used:
•	users.json  
•	brands.json  
•	receipts.json
### Approach:
•	Load JSON data using Python (pandas and json modules)  
•	Flatten the nested JSON structure  
•	Generate Metadata for each JSON file to understand the structure  
•	Define a relational schema based on the extracted insights and draft an ER diagram using draw.io tool
________________________________________
## Generate a query that answers a predetermined business question
After reviewing the JSON data, I created a relational schema. Using this relational data model, SQL queries are constructed which answer the following business questions, I have used MySQL dialect. Also, I have performed a few data cleaning tasks such as converting date fields from milliseconds to a standard timestamp, validated for null values, duplicate records, and incorrect relationships, as part of this, since data should be clean and have structured relationships, format to import into MySQL database.  
•	What are the top 5 brands by receipts scanned for most recent month?  
•	How does the ranking of the top 5 brands by receipts scanned for the recent month compare to the ranking for the previous month?  
•	When considering average spend from receipts with 'rewardsReceiptStatus’ of ‘Accepted’ or ‘Rejected’, which is greater?  
•	When considering total number of items purchased from receipts with 'rewardsReceiptStatus’ of ‘Accepted’ or ‘Rejected’, which is greater?  
•	Which brand has the most spend among users who were created within the past 6 months?  
•	Which brand has the most transactions among users who were created within the past 6 months?
________________________________________
## Generate a query to capture data quality issues against the new structured relational data model
Developed python scripts that can identify and capture data quality issues in the structured relational data model.
Example data quality issues addressed include:  
•	Missing values in critical fields.  
•	Invalid data formats.  
•	Duplicates or inconsistent data.  
•	Out-of-range values
________________________________________
## Write a short email or Slack message to the business stakeholder
Constructed an email to communicate all the findings to the business stakeholder clearly. Also, answered the following questions:  
•	What questions do you have about the data?  
•	How did you discover the data quality issues?  
•	What do you need to know to resolve the data quality issues?  
•	What other information would you need to help you optimize the data assets you're trying to create?  
•	What performance and scaling concerns do you anticipate in production and how do you plan to address them?
________________________________________
## Conclusion
This project demonstrates best practices in data modeling, SQL querying, and business communication. The structured approach ensures improved data accuracy, efficient queries, and better decision-making.




