
## Bank of America Consumer Complaint Analysis Report 

## **Table of Contents**

1.	[Introduction](#introduction)
2.	[Project Aim](#project-description)
3.	[Tools](#project-aim)
4.	[About the Dataset](#about-the-dataset)
5.	[Preparation of Dataset: Cleaning and Transforming](#preparation-of-the-dataset-cleaning-and-transforming) 
6.	[Data visualization in Power BI](#data-visualization-in-powerBI)
7.	[Insight from Data Analysis](#insights-from-the-data-analysis)
8.	[Recommendations](#recommendations-from-the-data-analysis)
9.	[Conclusion](#conclusion)


---
## 🚀 **Introduction**   
The banking industry in the U.S is one of the largest and most customer-driven service sectors. With thousands of consumers interacting with financial products everyday, customer satisfaction and complaint resolution have become critical metrics for maintaining trust and competitiveness. 
   Bank of America, as one of the largest banks , receives a significant number of consumer complaints filed through the Consumer Financial Protection Bureau (CFPB). This data presents an opportunity to understand pain points and improve service delivery.



---
## 🏦 **Project Description** 
This project focuses on analyzing operational, financial, and customer data from Bank of America to extract actionable insights for data-driven decision-making. Using Power BI, the dataset imported from Excel was transformed and visualized to understand patterns in consumer complaints, transaction behaviors, account activities, and financial trends.

The analysis aims to provide insights that can support various stakeholders, including:

Management:  Optimize operations and make strategic decisions.

Operations & Customer Service Teams:  Improve efficiency and enhance customer experience.

Regulators / Oversight Bodies:  Ensure compliance and monitor performance.

Customers / Public:  Understand trends and improve engagement.

---
## 🎯 **Project Aim** 

- The aim of this project is to analyze customer service and complaint data to answer critical business questions:

- Product Satisfaction: Which products generate the most customer dissatisfaction?

- Recurring Issues: What are the common complaints or issues that keep recurring?

- Complaint Channels: Which complaint channels (web, phone, etc.) are most effective in resolving issues?

- Response Timeliness: Are customer complaints responded to in a timely manner, and what happens when responses are delayed?


  ---
## 🛠 **Tools & Technologies** 

Power BI: Data visualization and dashboard creation.

Excel: Data source and initial storage.

---
## 📂 **About the Dataset** 
This dataset contains customer complaints submitted to the Consumer Financial Protection Bureau (CFPB) against Bank of America. It was imported from Excel into Power BI for visualization and analysis.

Each record represents a single complaint and contains key details about the product, issue, response, and resolution timeline.

Field	Description
- Complaint ID:	The unique identification number for a complaint.
- Submitted via:	How the complaint was submitted to the CFPB (e.g., Web, Phone, Email).
- Date submitted:	The date the CFPB received the complaint.
- Date received:	The date the CFPB sent the complaint to the company.
- Product:	The type of product the consumer identified in the complaint.
- Sub-product:	The type of sub-product the consumer identified in the complaint (not all Products have Sub-products).
- Issue:	The issue the consumer identified in the complaint (possible values are dependent on Product).
- Sub-issue:	The sub-issue the consumer identified in the complaint (possible values are dependent on Product and Issue, and not all Issues have corresponding Sub-issues).
- Company public response:	The company's optional, public-facing response to a consumer's complaint (e.g., "Company believes complaint is the result of an isolated error.").
- Company response to consumer:	This is how the company responded (e.g., "Closed with explanation.").
- Timely response?:	Whether the company gave a timely response (Yes/No).
- Customer Experience Teams: Understand behavior to improve satisfaction and retention.


  ---
  ## 🧹 **Preparation of Dataset: Cleaning and Transformation** 

Before building the dashboard in Power BI, the dataset was carefully prepared and transformed to ensure accuracy and reliability of the analysis. The following steps were performed:

1️⃣ Importing the Dataset

The dataset containing Bank of America customer complaints (sourced from CFPB) was imported from Excel into Power BI.

Verified all columns and data types (dates, text, numbers) on import to ensure compatibility with Power BI.

2️⃣ Data Preparation

Confirmed that the dataset contained no duplicate records — each Complaint ID was unique.

Ensured date fields (Date submitted and Date received) were correctly formatted as date values.

Standardized categorical values (e.g., “Yes/No” for Timely response?) for consistency across visuals.

3️⃣ Data Transformation

Created calculated columns to extract Year, Month, and Quarter from the Date submitted and Date received columns for time-trend analysis.

Grouped Products to simplify analysis and identify which product categories generated the most dissatisfaction.

Grouped Issues to identify recurring complaints and track patterns across products.

Created hierarchies (Product → Sub-product → Issue → Sub-issue) to enable drill-down in Power BI dashboards.

Added response performance metrics (e.g., Timely vs. Non-Timely responses) for stakeholder insights.

4️⃣ Data Model Setup

Established a clean, structured data model within Power BI to support interactive dashboards.

Ensured relationships between fields (e.g., Product, Issue, Channel, Date) were optimized for visualizations.


---
## 📊 **Data Visualization in Power BI** 

Two interactive dashboards were created:

1️⃣ Consumer Complaint Overview

KPIs: Total Complaints, Top Product Complaint, Recurring Issues, Timely Response Rate.

Most Recurring Issue: Bar chart showing top complaint categories.

Most Dissatisfied Products: Bar chart ranking products by complaint count.

Best Complaint Channel: Donut chart showing share of complaints by submission channel (Web, Phone, etc.).

Timeline of Customer Complaint: Area chart displaying trends over time.

2️⃣ Consumer Response & Outcomes

KPIs: Total Complaints, Average Resolution Time, Complaints from Web, Timely Response Rate.

Response Timeliness by Channel: Bar chart comparing timely vs. untimely responses across channels.

Complaint Resolution Outcomes: Bar chart showing types of company responses (public or private).

Trend of Timely Response: Area chart tracking response timeliness over months.

🔹 Interactivity

Filters for Month, Channel, Product, Company Response, and Timely Response to explore the data.

Drill-down from product to sub-product to issue to sub-issue.


---
## 🪞 **Insights from the Analysis**

The analysis conducted using Power BI provided answers to the business questions and revealed actionable insights about customer complaints at Bank of America:

1. Products Generating the Most Dissatisfaction

- Credit reporting and mortgage-related products recorded the highest number of complaints.

- Credit cards and checking accounts followed closely, showing key areas needing improvement in service delivery.

2. Recurring Issues

- The most frequently recurring issues include incorrect credit information, loan servicing errors, and billing disputes.

- These patterns suggest the need for better quality control, error resolution, and proactive communication with customers.

3. Most Effective Complaint Channels

- Most complaints were submitted via the web channel, indicating a preference for online communication by customers.

- Phone and other channels had comparatively lower submissions, suggesting that enhancing the web complaint system will directly benefit customers.

4. Timeliness of Responses

- A large majority of complaints received a timely response. However, a significant minority of cases did not, which correlates with higher dissatisfaction levels.

- Improving response speed could boost customer trust and reduce escalations.

5. Company Responses

- While many complaints were resolved with explanations or monetary relief, there is a notable portion where the company responded but chose not to make the response public.

- This lack of transparency can negatively impact customer perception and trust.


  ---
  
## **Recommendations by Stakeholder Group**

### (i) For Management / Executives 👔  
- 💰 Allocate resources to address account management issues, which are the top driver of complaints.  
- 🤖 Invest in process automation and customer support training to reduce complaint resolution times.  
- 📢 Increase public disclosure of complaint outcomes to build transparency and trust.  

### (ii) For Operations & Customer Service Teams 🛠️  
- 🖥️ Strengthen web complaint handling (staffing, monitoring, faster ticket resolution).  
- 👥 Develop issue-specific task forces (e.g., a team for account-management complaints).  
- 📊 Track KPIs regularly to sustain or improve the 94% timely response rate.  

### (iii) For Regulators / Oversight Bodies 🏛️  
- 🤝 Collaborate with CFPB to share improvement metrics and demonstrate progress on key issues.  
- 📝 Publish periodic customer satisfaction reports to enhance accountability.  

### (iv) For Customers / Public Stakeholders 🌐  
- 🗣️ Provide clearer communication on complaint progress.  
- 🔧 Improve self-service options for account management problems on the web portal.  


---
## **Conclusion**   
This project provides a data-driven view of consumer complaints lodged against Bank of America from 2017–2023. The analysis identified the products and issues generating the highest dissatisfaction, highlighted recurring complaint patterns, and evaluated the performance of response channels and timeliness.

By translating these findings into actionable recommendations, this work offers Bank of America a clear path to strengthen its complaint management process, streamline operations, and increase transparency. Implementing these measures would not only reduce complaint volumes but also enhance customer trust and loyalty over time.



