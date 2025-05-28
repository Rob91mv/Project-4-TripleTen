
# Megaline Phone Plans Analysis

![](https://www.nine.com.au/product-reviews/tech/how-to-choose-mobile-phone-plan-what-to-consider-everything-to-know/687c8f21-bacb-4343-8e0d-fb7bec6d3277)
## Project Overview:

As an analyst for the telecommunications operator Megaline, this project focuses on comparing the revenue performance of two prepaid plans, Surf and Ultimate. Using a dataset of 500 customers from 2018, which includes details such as calls, messages, internet traffic, and locations, the analysis aims to identify the plan that generates the most revenue. Data cleaning and preprocessing will be followed by visual analyses—such as histograms and boxplots—and statistical hypothesis testing to ensure robust conclusions.

## Data Dictionary:
- Users:
| Variable     | Description                                                                                |
|--------------|--------------------------------------------------------------------------------------------|
| user_id      | Unique user identifier                                                                      |
| first_name   | User's first name                                                                           |
| last_name    | User's last name                                                                            |
| age          | User's age (in years)                                                                       |
| reg_date     | Subscription date (dd, mm, yy)                                                              |
| churn_date   | Date when the user stopped using the service (if absent, the plan was active at extraction) |
| city         | User's city of residence                                                                     |
| plan         | Name of the plan used  

- Calls:

| Variable     | Description                               |
|--------------|-------------------------------------------|
| id           | Unique identifier of the call             |
| call_date    | Date of the call                          |
| duration     | Duration of the call (in minutes)         |
| user_id      | Identifier of the user who made the call  |

- Messages:

| Variable     | Description                                  |
|--------------|----------------------------------------------|
| id           | Unique identifier of the SMS                 |
| message_date | Date of the SMS                              |
| user_id      | Identifier of the user who sent the SMS      |

- Internet:

| Variable     | Description                                                             |
|--------------|-------------------------------------------------------------------------|
| id           | Unique identifier of the session                                        |
| mb_used      | Volume of data used during the session (in megabytes)                   |
| session_date | Date of the web session                                                 |
| user_id      | Identifier of the user who initiated the session                        |

- Plans

| Variable              | Description                                                                                       |
|-----------------------|---------------------------------------------------------------------------------------------------|
| plan_name             | Name of the plan                                                                                  |
| usd_monthly_fee       | Monthly fee in US dollars                                                                         |
| minutes_included      | Minutes included per month                                                                        |
| messages_included     | SMS included per month                                                                            |
| mb_per_month_included | Data included per month (in megabytes)                                                            |
| usd_per_minute        | Price per minute after exceeding the package limits                                               |
| usd_per_message       | Price per SMS after exceeding the package limits                                                  |
| usd_per_gb            | Price per gigabyte of additional data after exceeding the package limits (1 GB = 1024 megabytes)  |

## Impact:
The analysis of Megaline’s customer data has revealed important insights regarding usage patterns and revenue generation for its two prepaid plans: Surf and Ultimate. Through data consolidation and rigorous validation, a single database was created that captured monthly activity for calls, messages, and internet usage, as well as the costs associated with exceeding plan limits.

Statistical tests confirmed that average monthly revenues for the Ultimate plan are significantly higher than those for the Surf plan, despite Surf users frequently incurring extra charges for exceeding plan limits. This indicates that while the Surf plan generates additional revenue through over-usage, the overall financial benefit to Megaline is greater with Ultimate subscribers, who also demonstrate a clear preference for increased internet use.

Further, revenues in the New York–New Jersey region were found to be statistically different and higher compared to other cities. In practical terms, this suggests regional variations in customer behavior and spending power that may warrant tailored marketing strategies. These findings directly inform Megaline’s advertising budget allocation and highlight the Ultimate plan as the primary driver of overall revenue growth.

"TripleTen" Proyect #4 
