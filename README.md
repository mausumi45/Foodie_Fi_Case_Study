# Case-Study-3---Foodie-Fi
It's the 3rd Case study of 8 week SQL challenge of Data with Danny
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/00b67ec7-e4ef-499f-9436-67fbf9f661b8)
### Introduction:
Subscription-based businesses are super popular and Danny realized there was a large gap in the market - he wanted to create a new streaming service that only had food-related content - something like Netflix but with only cooking shows! 
Danny found a few smart friends to launch his new startup Foodie-Fi in 2020 and started selling monthly and annual subscriptions, giving their customers unlimited on-demand access to exclusive food videos worldwide!
Danny created Foodie-Fi with a data-driven mindset and wanted to ensure all future investment decisions and new features were decided using data. This case study uses subscription-style digital data to answer important business questions.

#### Available Data:
Danny has shared the data design for Foodie-Fi and also short descriptions of each of the database tables - our case study focuses on only 2 tables but there will be a challenge to create a new table for the Foodie-Fi team.
All datasets exist within the foodie_fi database schema - be sure to include this reference within your SQL scripts as you start exploring the data and answering the case study questions.

### ER Diagram:
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/b5c7fa9b-1a33-43e7-b8c0-bc7eb172c69e)

### Table-1 (Plans):
Customers can choose which plans to join Foodie-Fi when they first sign up.
Basic plan customers have limited access and can only stream their videos and is only available monthly at $9.90
Pro plan customers have no watch time limits and are able to download videos for offline viewing. Pro plans start at $19.90 a month or $199 for an annual subscription.
Customers can sign up to an initial 7 day free trial will automatically continue with the pro monthly subscription plan unless they cancel, downgrade to basic or upgrade to an annual pro plan at any point during the trial.
When customers cancel their Foodie-Fi service - they will have a churn plan record with a null price but their plan will continue until the end of the billing period.

### Table 2(subscriptions):
Customer subscriptions show the exact date where their specific plan_id starts.

## Case Study Questions:
This case study is split into an initial data understanding question before diving straight into data analysis questions before finishing with 1 single extension challenge.

#### A. Customer Journey
Based off the 8 sample customers provided in the sample from the subscriptions table, write a brief description about each customer’s onboarding journey.

Try to keep it as short as possible - you may also want to run some sort of join to make your explanations a bit easier!
#### Solution:
![A -Customer-Journey](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/615d5221-ffa6-434d-9b2a-a3576714d8aa)

### B. Data Analysis Questions:
#### 1. How many customers has Foodie-Fi ever had?
##### Solution :
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/d95e7287-3514-40d9-8044-1c1067865632)
#### 2. What is the monthly distribution of trial plan start_date values for our dataset - use the start of the month as the group by value
##### Solution:
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/d729f016-22f4-413e-8ed7-6c0019c70b8f)

#### 3. What plan start_date values occur after the year 2020 for our dataset? Show the breakdown by count of events for each plan_name
##### Solution:
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/fad27d1a-a305-47a4-848a-c430358dcc64)
#### 4.What is the customer count and percentage of customers who have churned rounded to 1 decimal place?
##### Solution:
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/0d59e21a-06d6-4111-b6ca-bfddae319660)

#### 5.How many customers have churned straight after their initial free trial - what percentage is this rounded to the nearest whole number?
##### Solution:
![image](https://github.com/user-attachments/assets/32b0ab83-5cc0-4b9b-a407-5d701ce5bab6)

#### 6.What is the number and percentage of customer plans after their initial free trial?
Solution :

#### 7.What is the customer count and percentage breakdown of all 5 plan_name values at 2020-12-31?

#### 8.How many customers have upgraded to an annual plan in 2020?

#### 9.How many days on average does it take for a customer to an annual plan from the day they join Foodie-Fi?

#### 10.Can you further breakdown this average value into 30 day periods (i.e. 0-30 days, 31-60 days etc)

#### 11.How many customers downgraded from a pro monthly to a basic monthly plan in 2020?
