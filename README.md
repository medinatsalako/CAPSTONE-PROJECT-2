# CAPSTONE-PROJECT-2

### PROJECT TITLE : Customer data 
[PROJECT OVERVIEW](#project-overview)
[DATA SOURCES](#data-sources)
[TOOLS](#tools)
### PROJECT OVERVIEW 

This project focuses on analyzing customer data to gain insights into subscription behaviour, revenue patterns and customer retention across various regions.

### DATA SOURCES    
The data used here was provided by the facilitatos.

### TOOLS
The tools used for this project are ;
- Microsoft Excel for data cleaning 
- SQL for data Querying
- Power Bi for visualisations  


### EXPLORATORY DATA ANALYSIS 
EDA was uses to answer the following 
- what is the overall customer behaviour
- what is the most preferred/popular subscription type
- what subscription type generates the peak revenue

  ### DATA ANALYSIS
  Below is a pictorial representation of the exploration analysis done with pivot table in Excel

 ![Screenshot (33)](https://github.com/user-attachments/assets/5c2e5a6e-08ea-4890-bd78-10fa657a9bc4)
  
![Screenshot (36)](https://github.com/user-attachments/assets/56d38afc-9174-4ae0-b89e-ab467931a663)

Below are some of the syntaxes used in SQL for quering data. 
- To get the average subscription duration 
- To get the total number of customers by region
 
```sQL
select AVG(datediff(day,subscriptionstart,subscriptionend))
 as AverageSubscriptionDuration
 from [dbo].[CUSTOMER DATA ]
 where subscriptionend is not null


 select region,
 count(distinct customerid)
 as totalcustomers
 from [dbo].[CUSTOMER DATA ]
 group by region
```

 

A pictorial representations of the queries used for the project in SQL


![Screenshot (37)](https://github.com/user-attachments/assets/5b50cdf2-7430-4248-bc95-d97dec1d515f)


![Screenshot (38)](https://github.com/user-attachments/assets/127007fe-374f-41a1-babe-b9a67aab0acd)


![Screenshot (39)](https://github.com/user-attachments/assets/8b1034f7-4214-4ca8-884d-aea824958809)


![Screenshot (40)](https://github.com/user-attachments/assets/7fc9085b-ea4a-42af-a551-44c49fbda6a8)
