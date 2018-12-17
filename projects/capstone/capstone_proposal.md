# Machine Learning Engineer Nanodegree
## Capstone Proposal
Siam Wannakosit  
October 29th, 2018

## Proposal

### Domain Background

Dtac application is one of Thailand’s large and fastest-growing mobile self-service channel for telecomunication in Thailand, connecting over 21 million users. dtac application is a self-service application which dtac prepaid and postpaid subscribers can use e-Services to check their call, value-added service (VAS) charges and VAS packages. In addition, the subscribers can also check rate, promotion, actual usage and how to make an International Call and use dtac International Roaming services 

### Problem Statement

As markets have become increasingly saturated, companies have attempted to identify ways in which to improve customer loyalty, satisfaction, and retention. This approach is supported by modern database technologies (Google Firebase), which enable to obtain the knowledge of who the customers are, what customers usage application, what they have purchased, when they purchased it, and predictions on behavior. Predicting when user will leave a dtac app creates a unique opportunity to increase active user and revenue contribution(lifetime value). This project focuses on predicting app churn for all user.  The traditional solution is to predict high-propensity churners and address their needs via a concierge service, marketing campaigns, or by applying special dispensations. Churn prediction, or the task of identifying customers who are likely to discontinue use of a mobile app service, is an important and concern of the Telecom industry.
The aim of this project is to study and analyze customer churn prediction based on mobile app usage logs and user behavior with the help of Google BigQuery.

### Datasets and Inputs

This datasets are collected as transaction log most of the data field are automatically collect by Firebase SDK, In this project focusing on event_name which is represent by user behavior eg. login, reward redeem, screenview, topup, subscription package and payment.

The datasets are collected and provided by Google Firebase.

Input data fields

| Field name                                  | Type    | Mode     |
|---------------------------------------------|---------|----------|
| event_date                                  | STRING  | NULLABLE |
| event_name                                  | STRING  | NULLABLE |
| event_params                                | RECORD  | REPEATED |
| event_params.key                            | STRING  | NULLABLE |
| event_params.value                          | RECORD  | NULLABLE |
| event_params.value.string_value             | STRING  | NULLABLE |
| event_params.value.int_value                | INTEGER | NULLABLE |
| event_params.value.float_value              | FLOAT   | NULLABLE |
| event_params.value.double_value             | FLOAT   | NULLABLE |
| user_pseudo_id                              | STRING  | NULLABLE |
| user_properties                             | RECORD  | REPEATED |
| user_properties.key                         | STRING  | NULLABLE |
| user_properties.value                       | RECORD  | NULLABLE |
| user_properties.value.string_value          | STRING  | NULLABLE |
| user_properties.value.int_value             | INTEGER | NULLABLE |
| user_properties.value.float_value           | FLOAT   | NULLABLE |
| user_properties.value.double_value          | FLOAT   | NULLABLE |
| user_properties.value.set_timestamp_micros  | INTEGER | NULLABLE |
| user_first_touch_timestamp                  | INTEGER | NULLABLE |
| user_ltv                                    | RECORD  | NULLABLE |
| device                                      | RECORD  | NULLABLE |
| device.category                             | STRING  | NULLABLE |
| device.mobile_os_hardware_model             | STRING  | NULLABLE |
| device.operating_system                     | STRING  | NULLABLE |
| device.operating_system_version             | STRING  | NULLABLE |
| device.vendor_id                            | STRING  | NULLABLE |
| device.advertising_id                       | STRING  | NULLABLE |
| device.language                             | STRING  | NULLABLE |
| app_info.version                            | STRING  | NULLABLE |
| platform                                    | STRING  | NULLABLE |



### Solution Statement



_(approx. 1 paragraph)_

In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, describe the solution thoroughly such that it is clear that the solution is quantifiable (the solution can be expressed in mathematical or logical terms) , measurable (the solution can be measured by some metric and clearly observed), and replicable (the solution can be reproduced and occurs more than once).

### Benchmark Model
_(approximately 1-2 paragraphs)_

In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail.

### Evaluation Metrics

User Retention measures the stickiness of our dtac app, Increasing engagement and retention will lead to more active and loyal app users.  - that is, how often people engage with app. 
“stickiness” – how engaged and loyal users are for a dtac app. For those that are concerned primarily with user conversions and monetization, the most important objective is to keep users engaged and ensure repeat usage.


### Project Design
_(approx. 1 page)_

In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

-----------

**Before submitting your proposal, ask yourself. . .**

- Does the proposal you have written follow a well-organized structure similar to that of the project template?
- Is each section (particularly **Solution Statement** and **Project Design**) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
- Would the intended audience of your project be able to understand your proposal?
- Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
- Are all the resources used for this project correctly cited and referenced?
