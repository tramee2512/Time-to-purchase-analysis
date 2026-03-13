# E-Commerce Conversion Analysis: Same-Day Purchase Speed

## Overview

This analysis was conducted for an e-commerce product team within a web company operating across multiple industries. One of the company’s core business lines is an online store that regularly launches new features and analyses user behaviour to improve conversion performance and customer experience. As part of the Product Analytics function, I partnered with the Product Manager to investigate how long it takes users to complete their first purchase after arriving on the website on a given day.

For an e-commerce product team, conversion is not only about whether users purchase, but also how quickly they do so. The analysis focuses on same day purchase speed, defined as the duration between a user’s first website arrival and their first purchase on that same day. This metric reveals the pace of decision-making, highlights patterns that may influence checkout experience, marketing performance, and overall customer purchase behaviour.

To answer the business question, I used SQL to identify each user’s first arrival and first same-day purchase at the daily level, then analysed purchase duration trends over time and across key dimensions. The dashboard and presentation were designed around the daily progression of purchase duration, while also incorporating additional analysis to uncover meaningful behavioural patterns for product and commercial stakeholders.

To support decision-making, insights and recommendations are provided across the following key areas, enabling the Product, Marketing, and Design teams to better understand conversion behaviour and prioritise optimisation opportunities more effectively.
* **Purchase Speed Trends:** Measuring how quickly users convert after landing on the site and how this behavior evolves over time.
* **Device Performance:** Evaluating whether conversion speed differs across desktop, mobile, and tablet users.
* **Traffic Medium Analysis:** Assessing how acquisition channels influence purchase behavior.
* **User Behavior by Time of Day:** Understanding how purchase intent varies depending on when users visit the website.

## Executive Summary
Analysis of 4,793 same-day purchases between November 2020 and January 2021 shows that most users convert quickly after arriving on the website. The median purchase time is 19 minutes, with 41% of purchases occurring within 15 minutes and nearly 65% within 30 minutes. 

While typical purchase behavior is fast and consistent, conversion speed varies across devices, acquisition channels, and times of day. Desktop users generate the largest purchase volume but show longer conversion times, CPC traffic converts slower than organic traffic, and late night visitors tend to take significantly longer to complete purchases.

These findings highlight opportunities to optimize checkout flow, marketing targeting, and engagement strategies to improve conversion efficiency.
________________________________________
## Key Metrics 
The analysis focuses on several metrics to evaluate how quickly users convert after arriving on the website and to understand patterns in purchase behaviour.

•	**Purchase Duration:**
The time (in minutes) between a user’s first website arrival of the day and their first purchase on the same day. This is the primary metric used to measure conversion speed.

•	**Median Purchase Duration:**
The median time it takes users to complete a purchase. Median is used as the main indicator of typical user behaviour because it is less affected by extreme outliers.

•	**Average Purchase Duration:**
The average time between arrival and purchase. This metric helps highlight the influence of unusually long sessions and provides additional context when compared with the median.

•	**Purchase Volume:**
The total number of same-day purchases within the analysis period. This helps identify which user segments contribute most to overall conversions.

•	**Purchase Distribution by Segment:**
Comparison of purchase duration and purchase volume across dimensions such as device type, traffic source, and time of day to identify differences in conversion behaviour.

## Deep-Dive Insights
**1. Most Purchases Occur Shortly After Site Arrival**

Users typically convert quickly after landing on the website. The median purchase duration is 19 minutes, and nearly two-thirds of purchases occur within 30 minutes of the first visit. 

However, the average purchase duration is significantly higher due to extreme outliers, with the longest recorded duration exceeding 1,400 minutes. These outliers distort the average metric, making the median a more reliable indicator of user behavior.

This suggests that when users decide to purchase, they tend to do so quickly, and delays in the funnel may indicate friction points or exploratory browsing.

**2. Purchase Speed Is Consistent Over Time**

The median purchase duration remains relatively stable across the three-month period analyzed. While average purchase time fluctuates due to extreme outliers, the typical conversion journey does not show major behavioral changes.

This indicates that the existing purchase funnel performs consistently and that improvements should focus on reducing friction rather than addressing structural changes in user behavior.

**3. Desktop Drives the Largest Purchase Volume**

Desktop users generate the largest number of purchases (2,716 transactions), followed by mobile (1,974) and tablet (103).  However, desktop sessions also show longer and more variable purchase durations, suggesting that desktop users may spend more time researching or comparing products before purchasing.
 Optimizing the desktop checkout experience could therefore have the greatest impact on improving overall conversion speed.

**4. Traffic Source Influences Conversion Behavior**

Acquisition channels show noticeable differences in purchase speed. Organic traffic produces the highest purchase volume with relatively fast conversion times, indicating strong user intent. In contrast, CPC traffic converts more slowly, suggesting that paid campaigns may attract lower-intent users or direct users to less optimized landing pages.


**5. Time of Day Affects Purchase Speed**

User purchase behavior varies depending on the time of day. Visitors arriving during late-night hours take significantly longer to complete purchases, suggesting lower purchase intent during these periods. Daytime visitors tend to convert faster, indicating stronger purchasing intent and more focused browsing behavior.

## Recommendations
**1. Improve Desktop Checkout Experience**

Desktop generates the highest purchase volume but also shows longer purchase durations. Improving the desktop checkout flow could reduce friction and accelerate conversion. Potential improvements include:
- Reducing the number of checkout steps
- Improving autofill and payment flow
- Optimising page performance and load times
- Adding reminders or prompts for incomplete carts

**2. Optimize Paid Acquisition Channels**

Users arriving through CPC channels appear to convert more slowly than those from organic sources, which may indicate lower purchase intent or weaker landing page alignment.
The Marketing team should:
- Review campaign targeting and audience quality
- Improve landing page relevance and messaging alignment
- Reallocate budget toward higher-performing channels if needed

**3. Prioritize High-Intent Traffic Sources**

Organic channels appear to deliver faster conversion behaviour than paid acquisition channels, suggesting that users arriving through organic search often have stronger purchase intent. These visitors are more likely to land on the website after actively searching for specific products or solutions, which shortens the time needed to complete a purchase. Strengthening SEO and other organic acquisition strategies could therefore attract more high-intent users, reduce time-to-purchase, and improve overall conversion efficiency.

**4.Align Marketing Efforts with High-Intent Time Periods**

Purchase speed appears to vary by time of day. Since users tend to convert faster during daytime hours, marketing campaigns and promotions may perform better when scheduled during these periods.
Potential actions include:
- Prioritising campaigns during high-intent daytime hours
- Testing reminders or re-engagement strategies for night-time visitors

**5. Improve Traffic Source Tracking**

Some purchases are labelled as “Unknown” traffic source, meaning the system cannot identify how those users arrived at the website. This makes it harder to accurately evaluate which marketing channels are driving conversions. Improving campaign tracking would provide clearer insights into channel performance and help the business make better decisions about marketing investment.

## Expected Business Impact
If implemented, these improvements could help increase conversion efficiency and improve the overall purchase experience:

- **Faster Checkout Experience:**
Simplifying the desktop checkout flow and reducing friction may shorten purchase duration and increase completed transactions, especially for high-volume desktop users.

- **Improved Marketing Efficiency:**
Refining CPC targeting and prioritising high-performing acquisition channels could attract users with stronger purchase intent and improve return on marketing investment.

- **Higher Conversion from High-Intent Traffic:**
Strengthening organic acquisition strategies may increase the share of users who convert quickly after arriving on the site.

- **Better Timing of Marketing Campaigns:**
Aligning promotional activities with higher-intent daytime periods may improve engagement and conversion outcomes.

- **More Reliable Performance Insights:**
Improving tracking and attribution will enable more accurate analysis of channel performance, supporting better data-driven decisions across product and marketing teams.

## Limitations
Several limitations should be considered when interpreting these findings:
- The analysis includes only same-day purchases, excluding users who return on later days to complete transactions.
- New and returning users are not segmented.
- Product type and order value are not considered, making it difficult to assess whether longer purchase durations correlate with higher value purchases. 

These limitations mean the results should be interpreted as general behavioural patterns rather than precise performance benchmarks.

## Future Analysis
Further analysis could provide deeper insights into user purchasing behavior:
- **Cohort Segmentation** to compare behavior between new vs returning buyers.
- **Multi-Day Conversion Analysis** to capture delayed purchases.
- **Revenue Weighted Conversion Analysis** to incorporate order value.
- **Outlier Investigation** to understand whether extremely long purchase durations
are caused by technical issues, complex purchasing journeys, or research driven customers.
- **A/B Testing** to measure the impact of checkout improvements on conversion speed.

## Tools Used
- **BigQuery SQL:** data extraction and transformation.
- **Power BI:** dashboard development and visual storytelling.
- **PowerPoint:** stakeholder presentation of findings and recommendations.
