# upGrad-TelecomChurnCaseStudy

# Problem Statement

This is a student exercise using telecom churn data. The goal is to build a model to predict customer churn probability. The data is provided in two parts: one dataset with known churn outcomes (`train.csv`) and another without churn outcomes (`test.csv`).

### Exercise Overview:

1. **80% weightage:** Focus on building the best model for the business case—predicting churn probability based on multiple KPIs.
2. **20% weightage:** A submission to a Kaggle competition, where the model is evaluated on unseen data (`test.csv`).

The data contains KPIs measured across months, and our EDA will explore how these KPIs evolve over time. We will also test different models to compare their performance and choose the best one for Kaggle submission.

The model with the highest accuracy will be selected for the Kaggle submission, even if it is not the best across all evaluation metrics.

-------------------
# Data dictionary

|Acronyms|Description|
|---|---|
|CIRCLE_ID|Telecom circle area to which the customer belongs to|
|LOC|Local calls  within same telecom circle|
|STD|STD calls  outside the calling circle|
|IC|Incoming calls|
|OG|Outgoing calls|
|T2T|Operator T to T ie within same operator mobile to mobile|
|T2M    |Operator T to other operator mobile|
|T2O    |Operator T to other operator fixed line|
|T2F    |Operator T to fixed lines of T|
|T2C    |Operator T to its own call center|
|ARPU    |Average revenue per user|
|MOU    |Minutes of usage  voice calls|
|AON    |Age on network  number of days the customer is using the operator T network|
|ONNET   |All kind of calls within the same operator network|
|OFFNET    |All kind of calls outside the operator T network|
|ROAM|Indicates that customer is in roaming zone during the call|
|SPL   |Special calls|
|ISD    |ISD calls|
|RECH    |Recharge|
|NUM    |Number|
|AMT    |Amount in local currency|
|MAX    |Maximum|
|DATA    |Mobile internet|
|3G    |G network|
|AV    |Average|
|VOL    |Mobile internet usage volume in MB|
|2G    |G network|
|PCK    |Prepaid service schemes called  PACKS|
|NIGHT    |Scheme to use during specific night hours only|
|MONTHLY    |Service schemes with validity equivalent to a month|
|SACHET   |Service schemes with validity smaller than a month|
|*.6    |KPI for the month of June|
|*.7    |KPI for the month of July|
|*.8    |KPI for the month of August|
|FB_USER|Service scheme to avail services of Facebook and similar social networking sites|
|VBC    |Volume based cost  when no specific scheme is not purchased and paid as per usage|
-------------------
