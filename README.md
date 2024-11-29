# Project Background
Shopzilla, a leading e-commerce platform established in 2008, focuses on offering a diverse range of products, including electronics, apparel, and home essentials, connecting millions of customers to trusted sellers. With its customer-centric business model, Shopzilla relies heavily on exceptional customer service to enhance user experience and build trust among buyers and sellers. This project analyzed customer service interactions to identify key drivers of Customer Satisfaction (CSAT) and operational inefficiencies that impact service quality. The findings and recommendations aim to support the customer service and operations teams in improving service delivery, enhancing customer experience, and optimizing agent performance.

The project focused on two key objectives:

*   **Identifying Key Drivers of Customer Satisfaction:** This analysis examines critical factors such as response times, agent tenure, interaction categories, and shift timing to uncover the root causes of low CSAT scores. The goal is to identify actionable insights to address specific pain points and enhance the overall customer service experience.
*   **Optimizing Operational Efficiency**: The study evaluates operational metrics, including service channels, interaction timing, and manager performance, to pinpoint inefficiencies and implement workflow improvements. This ensures Shopzilla’s operations are streamlined to deliver consistent, high-quality customer support.

This analysis uncovered actionable insights into customer service performance and agent management, providing a foundation for targeted interventions to enhance both customer satisfaction and operational outcomes.

<br/>

The original dataset and Excel dashboard for this analysis is available here \[[link](https://github.com/KunLinTsai24/Excel--Customer-Satisfaction-Enhancement/tree/main/data)\]. 

# Data Structure & Initial Checks

The company’s database consists of 85K records, capturing records of customer interactions, categorized by various attributes such as shift timing, manager, tenure, channel, and issue category. Key data variables include:

- **CSAT Score:** Customer satisfaction rating for each interaction.
- **Channel Name:** Mode of customer service (e.g., Email, Inbound, Outcall).
- **Agent Shift:** Timing of the interaction (e.g., Morning, Evening).
- **Category:** Nature of the interaction (e.g., Cancellations, Product Inquiries).
- **Manager:** Supervisors responsible for team operations.
- **Tenure Bucket:** Categorized levels of agent experience.
- **Interaction Timeline Details:** Including timestamps for when the issue was reported, responded to, and the survey feedback was received.

Initial data checks identified some missing values in fields like **Customer Remarks, Customer city, Product category, Connected handling time, and Item price**, which were excluded due to insufficient data for analysis.

# Executive Summary

### Overview of Findings

The analysis highlights several key factors influencing customer satisfaction and operational performance. Response time emerges as a critical driver of CSAT, with faster resolutions (under 3 hours) significantly outperforming delayed responses. Agent experience also plays a pivotal role, as more experienced agents consistently achieve higher CSAT scores. Operationally, the email channel and morning shifts underperform compared to other channels and shifts, indicating targeted areas for improvement. Additionally, specific low-scoring interaction categories, such as cancellations and product inquiries, require enhanced resolution processes to address customer dissatisfaction effectively. Furthermore, the performance of managers shows a notable impact, with underperforming managers, such as Olivia Tan and William Kim, consistently recording lower CSAT scores, highlighting potential gaps in leadership or team management that affect overall service quality.

![](https://github.com/KunLinTsai24/Excel--Customer-Satisfaction-Enhancement/blob/main/img/Customer%20Satisfaction%20Dashboard.png)

# Insights Deep Dive

### Key Drivers of Customer Satisfaction

- **Faster Resolutions Drive Higher Scores:** Interactions resolved within 3 hours achieved an average CSAT score of 4.32, whereas issues resolved after 72 hours dropped significantly to 3.12. This highlights the critical role of swift response times in maintaining customer satisfaction.
- **Tenure’s Impact on Performance:** Agents with over 61-90 days of experience outperformed newer agents in training, achieving CSAT scores of 4.35 compared to 4.15. This underscores the value of agent expertise and the importance of comprehensive training programs.
- **Cancellations and Product Inquiries Lagging:** These categories recorded some of the lowest CSAT scores, with cancellations at 3.99 and product inquiries at 4.04. This suggests ongoing issues with resolution processes or a lack of effective communication, leading to customer dissatisfaction.

### Optimizing Operational Efficiency

- **Email Channel’s Poor Performance:** The email channel recorded the lowest CSAT score of 3.90, compared to inbound calls (4.25) and outbound calls (4.27). This indicates possible inefficiencies in written communication, delayed responses, or resolution clarity, requiring immediate attention.
- **Morning Shift Challenges:** The morning shift underperformed across all metrics, achieving a CSAT score of 4.19 compared to the evening (4.28) and night (4.29) shifts. Despite no noticeable difference in workload, this trend suggests readiness issues or operational gaps during morning hours.
- **Underperforming Managers:** Managers Olivia Tan and William Kim consistently scored the lowest, with CSAT scores of 4.11 and 4.12, respectively. This highlights potential leadership or team management issues impacting agent performance and customer satisfaction.

# Recommendations

- **Streamline Resolution Timelines:** Develop streamlined workflows and automated solutions to reduce response times, especially for complex issues that typically exceed 72 hours. This aligns with the insight that faster resolutions lead to significantly higher CSAT scores.
- **Enhance Agent Onboarding and Training:** Strengthen onboarding programs and provide continuous training for agents with less than 90 days of tenure. Focus on equipping them to handle low-scoring categories like cancellations and product inquiries, which are critical to improving customer satisfaction.
- **Revamp Email Support Systems:** Overhaul email handling processes by introducing response templates, improving email management systems, and providing agents with specialized training in written communication to address the channel’s low CSAT score.
- **Improve Morning Shift Readiness:** Conduct an in-depth review of morning shift operations to identify and resolve specific challenges, such as readiness, support resources, or scheduling. Implement strategies like pre-shift briefings and targeted performance support to enhance morning shift scores.
- **Provide Leadership Training for Underperforming Managers:** Offer targeted leadership development programs to managers with consistently low scores (e.g., Olivia Tan and William Kim). Focus on improving communication, team motivation, and management effectiveness to bridge leadership gaps and improve overall team performance.

# Assumptions and Caveats

- **Incomplete Customer Feedback Data:** Missing values in the "Customer Remarks" field were excluded from the analysis, as they provided insufficient information to assess customer sentiment or CSAT drivers effectively.
- **Equal Weighting of Categories:** The analysis treats each category within variables, such as interaction type or shift, as equally important without considering the differing volume or frequency of interactions across these categories, which may influence overall CSAT scores.
- **Simplified One-Dimensional Analysis:** The analysis focused on evaluating variables individually rather than exploring multi-dimensional relationships, potentially overlooking complex interactions between variables that might influence CSAT scores.
