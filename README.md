# Objective

In this project, a preliminary analysis of the rates of a carrier will be conducted based on a relatively small selection of customers. The behavior of the customers will be analyzed, and it will be determined which prepaid rate generates more revenue.

Below hypotheses will be tested:
 
1. The average income of users with Ultimate and Surf plans differs.
2. The average income of users in the New York-New Jersey area is different from users in other regions.

# Data

1. The users table:
* user_id - unique identifier of the user
* first_name - user's first name
* last_name - user's last name
* age - user's age
* reg_date - date of subscription 
* churn_date - the date when the user stopped using the service
* city - the user's city of residence
* plan - tariff name

2. calls table:

* id - unique identifier of the call
* call_date - date of the call
* duration - duration of the call (in minutes)
* user_id - the identifier of the user making the call

2. The messages table:

* id - unique identifier of the SMS
* message_date - date of SMS
* user_id - the identifier of the user sending the SMS

3. The internet table:

* id - unique session identifier
* mb_used - the volume of data spent during the session (in megabytes)
* session_date - date of the web session
* user_id - user identifier

4. plans table:

* plan_name - tariff name
* usd_monthly_fee - monthly payment in US dollars
* minutes_included - included minutes per month
* messages_included - SMS included per month
* mb_per_month_included - data included per month (in megabytes)
* usd_per_minute - price per minute after exceeding the package limits
* usd_per_message - price per SMS after exceeding the package limits
* usd_per_gb - price per gigabyte of extra data after exceeding the package limits

# Library

* Pandas
* Numpy
* Scipy
* Numpy

# Conclusions

To begin with, a data cleaning was carried out to prepare our dataset for analysis, duplicate values were eliminated, incomplete and null values were treated. Subsequently, a statistical analysis was performed to evaluate the behavior of the users of both plans, and the following was found:

1. There is a significant difference between the average earnings of users in New York-New Jersey and other regions.
2. The result of the statistical test indicates that the average revenue of users of the Ultimate and Surf calling plans is significantly different. This is because the p-value is much smaller than the typical alpha value of .05. Consequently, we can reject the null hypothesis and conclude that there is a statistically significant difference in the average revenue between Ultimate and Surf plan users.
3. The Ultimate plan produces higher revenues than the Surf plan.

This analysis provides us with an overview of the behavior of users regarding the different benefits of each plan and how their telephone consumption habits vary depending on their geographic area and the plan contracted.
