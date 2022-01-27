---
title: "Product Execution Problem : How to diagnose a Product Issue \n| The Great
  PM Interview"
image: assets/images/Great-PM-Interview-Product-Execution-RCA.jpg
author: tarun
categories: interviews
tags:
- Product Case Interview
- Product Execution
- The Great PM Interview
- Product Managers
- Job Interviews
- Problem Solving
- RCA
- Debugging
- Product Management
- featured
---

Product Execution Interview is highly relevant in the day to day execution job of a Product Manager. The problems given are analytical, strategy and goal focused.
One such product execution question is to debug an issue in a product, feature or KPI generally asked in FAANG/Big Tech Companies (Google, Facebook interviews). The interviewer explains some symptoms (like change in the metrics, feature or customer behaviour) and expects situational and the root cause analysis of the problem. These are referred as *"debugging", "investigation", "root cause", "metric change" or "diagnosis"* questions. Even in a typical work environment, PM and his team has limited time and resources to asses and react to such problems. Similar to a Doctor, PMs here try to -
* Understand the symptoms by asking questions
* Check the associated indicators
* Probe various causes and their probabilities by hit and trial method
* Eliminate the possibilities one by one to reach right root cause and at last
* Prescribe a solution

Rather than being a basic health diagnosis by a doctor, it is to be understood as case analysis by different medical experts in an OT (operation theater). PM leads the discussion between engineering, business, operations, data science PM in this case.

```
PROBLEM SOLVING : PRODUCT EXECUTION QUESTIONS

- An FB product shows a 10% drop in newly registered users: 
   what data would you need to understand and fix the problem?”
- You are PM of FB Login for 3rd parties & successful logins metrics is down, 
   what will you do?
- Imagine you were PM for buyer seller market-place; 
   what would be the key metric, how would you diagnose a drop. 
- Yelp customers tweeted about incorrect wait time in the waitlist feature. 
   How would you investigate? 
- One of our merchants is noticing an increase in fraud. 
   How would you solve the problem?
- You are the PM of Lyft, there is a sudden increase of users canceling rides. 
   How would you analyze and correct this?
- You ran A/B test. Page Engagement up but Newsfeed Engagement down.
   What will you do?
- LinkedIn's engagement is falling 10% day on day. 
   What would be your approach towards this ?
```

In this article, we will share an exhaustive approach with sample questions to ask the interviewer. Broadly, solving these questions involve 4 Steps

<p style="color: #EA2F65"> <b>
	
<img src="{{ site.baseurl }}/assets/images/Product_Execution_Question.png" 
		 alt="Product Execution Question"
     width="100%" 
     height="auto" />			
	
</b></p>

# 1) Clarify

<p style="color: #EA2F65"> <b> Understand the Issue/Metric</b></p>

Firstly, understand the question and the metric well. It is important so that you solve the right problem. Make sure that you reiterate the problem and the definition of the metric that has exhibited the change. 
E.g. - If the problem is "LinkedIn's engagement is falling 10% day on day...." First understand how is the engagement measured for Linkedin if it is not clear. 


```
CLARIFYING QUESTIONS TO ASK :-

How do we define the metric ?
Is it an absolute or %age change in the metric ?
What is the period in which change is observed ? Is it over a day or week over week ?
What is the Baseline? Do we already know what this change is high or low ?
Do we consider this highly urgent or critical in terms of impact ?
```

<i>Pro Tip :- <br>
#You can also state your understanding with an assumption e.g. "User Engagement at linkedin which I assume is cumulatively measured in terms of number of post views, likes, shares and comments from the linkedin users, is dropping at the rate of 10% per day"
	</i>
	

# 2) Explore

<p style="color: #EA2F65"> <b> Analyse the Situation - Ask probing questions</b></p>

Understanding the situation and context requires exploring both internal factors and external factors. 
Internal factors are mostly within the team's control while external factors are outside their control. Generally, this approach is both mutually exclusive and exhaustive and hence saves time to debug. Communicate your approach and questions to the interviewer so that he could guide you to more information and help you identify the cause.

<u><i>Internal Factors</i></u>

During an actual on-job scenario, a PM will generally first probe into the below internal factors.
* Data - funnel measurement, data errors, related metrics
* Timeline - sudden change vs long term trends, seasonality
* User - customer segments, feedback, social noise
* Product - geography, channel, related features
* Technology - bugs, new deployment

```
CLARIFYING QUESTIONS TO ASK :-

Data
What is the impact to the key or North Star metrics - engagement, user traffic ?
Have we analysed  funnel metrics ? Bot traffic more or less?
How are demand or supply metrics ?
Is it possible that we've measured the metric incorrectly?

Timeline 
Is the change one-time event or occurred in the past or progressively ? 
When is the issue first detected and since when it is actually happening ?
Do we see any seasonality trend ? Has it happened over Peak/Christmas/holidays ?

Users
What is the impact to the overall user journey (from acquisition to satisfaction) ?
Does data suggest that the issue is with a customer segment ? New ? Paid or free ?
Have we got any User reviews and social media feedback ?

Product
What is the phase of the product ? mature or new ?
Is it happening across all geographies or any region ? Language ? new launch ?
Is it happening for some or all channels or categories ?
Is there any visible change in metrics of any other features ? 
- Payment service ? Recommendation/Feed/Search/CTAs ?
Is the decline happening on specific platforms, like iOS, Android, Web or others? 
Is this happening on browsers or phone models ? 
A new feature launch/change ? Product change by any Product-Engineering team ? 
Any changes in product marketing ?

Technology
Have we done any deployment recently ? 
Was there a downtime, outage, delays, service alert, Load time ?
Have we identified any bug that could impact the change ?
Is there any technology/service (Cloud, ML, SEO/SEM) facing an outage
```

<u><i>External Factors</i></u>

After checking the internal factors, we will move to the below external factors. 
* Industry  
* Competitors
* User behaviour
* Society or Environment

```
CLARIFYING QUESTIONS TO ASK :-

Is there an Industry trend we should be aware of ? Any impact on Competitors ?
Is there any competitor taking market share ?
Any new launch/announcement/news from competitors ?
Are there any Macro economic factors like covid ? Holiday/ Sports/ Strike/ Disaster
Any long term change in the target user's behaviour (e.g. online deliveries) ?
Any outage with 3rd party service or platform provider (e.g. Cloud, Appstore) ?
``` 


<i>Pro Tip :- <br>
#To be comprehensive, it is best to go through the external factors anyway even if you found some probable internal causes already. 
	</i>
# 3) Hypothesize
<p style="color: #EA2F65"> <b> Postulate the Probable Causes </b></p>

Now that you have gathered all the information, synthesize the information and build some hypothesis to test. Prioritize the hypothesis to be validated and share your reasons.
You can use a phrase like - “Let me build some hypothesis to test and identify the cause”. 
State the assumption based on the identified information e.g. “Let's assume that the algorithm which decides public events are shown/recommended to a user in their Event page changed"

Test the Hypothesis with data by checking
* Customer feedback - App reviews, CS tickets, Social media mentions
* Logs, Crash reports, Network activity - dos attack, Data centre
* Related KPIs
* Traffic metrics and conversion funnel
* Notifications/marketing comms
* Market data


```
COMMON ROOT-CAUSES :-

Look for Drop in funnel - overall traffic to conversation
Bugs or new launches - Recommendation/Feed/Search/CTAs
Channel issue - organic search, referral, direct, new customer, repeat customers
Platform Issue - IOS, Android, Mweb, Web
Category issue - "No. of Customer Returns in Shoes/Apparels"
Check customer segments - New vs Old
Feature deployment, App updates, A-B testing, UI change, privacy settings
Data instrumentation/Reporting issues 
Trends in Market or User Dynamics - user-friendly payment options
Calamities - International Supply challenge, Natural disaster, Covid, Football match
``` 

<i>Pro Tip :- <br>
#While PMs validate the hypothesis in a real situation, they also inform all partner teams (business, technology, operations, data, customer service teams) based on the impact and urgency. They request for any additional information or feedback from the teams.  
	</i>
	
# 4) Conclude

<p style="color: #EA2F65"> <b> Summarize with Recommendation </b></p>

 
Finally, conclude with Summary and recommend course of actions. Emphasize that you have ruled out other causes with reasonable confidence and will continue to monitor and probe further till we resolve this. Prioritize and recommend the set of feature/fix for resolution.  Communicate the tradeoffs if any.

```
COMMON ACTIONABLES :-

Check UI/flow myself
Start impact analysis
Hotfix
Roll back
Search, Recommendations or other Data Science algorithms
Align Business/Product teams on trade-offs
```
