---
title: 'Analyzing booking conversion funnel : Case Study - Ola Cabs'
categories: analytics
author: tarun
image: assets/images/booking-funnel-conversion.jpg
tags: featured
---

Product Managers and Analysts working on consumer facing products often dig into every click or interaction data in the core  flows like checkout or booking funnel. The objective is to not only optimize the conversion (and ofcourse growth) but also to find gaps in customer experience. Let's take below a basic example of user journey on Ola cab's App ( Ola cabs is leading cab aggregator in India with fierce competition with Uber). AIDA model ( Attention>Interest>Desire>Action ) is also used here for explaination.

Booking Funnel for individual Cab Categories ( like Micro, Mini etc ) can be measured in terms of app sessions or user clicks / unique users.

![Ola-booking-screens]({{ site.baseurl }}/assets/images/Ola-booking-screen.jpg)

The Key Metrics - 

* **Sum of All App sessions** ( User Awareness/intent on platform )
* **Sum of category "Ride now"** button click sessions ( User Desire )
* **Sum of category "Confirm"** button click sessions ( User Action )
* **Sum of category "Ride Scheduled"** sessions ( Booking requested )
* **Sum of category "Rides Completed"** ( Booking confirmed )

Below is the snapshot of the possible leakages across each step in the flow

* **App sessions** \-->Drop offs due to no cab availability or poor ETAs
* **Ride now clicks**  \-->Drops offs due to ETA or availability or pricing
* **Confirm Button clicks**  \-->Drops offs due to pricing or errors
* **Rides Scheduled**  \-->Drops offs due to stockouts
* **Rides completed**  \-->Driver and Customer cancellations

Hope this basic example helps with a basic framework for analysing and optimizing App or web flows/funnels