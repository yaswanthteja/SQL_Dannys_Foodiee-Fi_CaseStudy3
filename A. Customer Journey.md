# 🥑 Case Study #3 - Foodie-Fi

## 🎞 Solution - A. Customer Journey

Based off the 8 sample customers provided in the sample subscriptions table below, write a brief description about each customer’s onboarding journey.

<img width="261" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/images/A.Customer%20journey/Img1.png">

**Answer:**

````sql
SELECT
  s.customer_id,f.plan_id, f.plan_name,  s.start_date
FROM foodie_fi.plans f
JOIN foodie_fi.subscriptions s
  ON f.plan_id = s.plan_id
WHERE s.customer_id IN (1,2,11,13,15,16,18,19)
````

<img width="556" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/images/A.Customer%20journey/img2.png">
From the sample results, I will choose 3 customers and write about their onboarding journey.

<img width="560" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/images/A.Customer%20journey/img3.png">

Customer 1 started the free trial on 1 Aug 2020 and subsequently subscribed to the basic monthly plan on 8 Aug 2020 after the 7-days trial has ended.

<img width="512" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/images/A.Customer%20journey/img4.png">

Customer 13 started the free trial on 15 Dec 2020, then subscribed to the basic monthly plan on 22 Dec 2020. 3 months later on 29 Mar 2021, customer upgraded to the pro monthly plan.

<img width="549" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/images/A.Customer%20journey/img5.png">

Customer 15 commenced free trial on 17 Mar 2020, then upgraded to pro monthly plan on 24 Mar 2020 after the trial ended. In the following month on 29 Apr 2020, the customer terminated subscription and churned until the paid subscription ended on 24/25 May 2020.

***

Click here for [solution](https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3/blob/master/B.%20Data%20Analysis%20Questions.md) to **B. Data Analysis Questions**! 🙌🏻
