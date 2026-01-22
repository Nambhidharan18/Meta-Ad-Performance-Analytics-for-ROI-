## Meta Advertising Performance Analytics for ROI 

#### Description
Analyzed Facebook and Instagram advertising data to track campaign performance, measure conversions, and optimize budget allocation to improve marketing ROI(Return of Investment).



### 1. Introduction

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

Tracking advertising performance across Meta platforms is a critical challenge in digital marketing, as businesses must determine which campaigns effectively drive engagement and conversions. Without unified performance insights, marketing teams risk inefficient budget allocation and reduced return on investment. Data-driven analysis provides visibility into reach, engagement, conversion trends, and spend across Facebook and Instagram, enabling informed decision-making and continuous campaign optimization.


### 2. Problem Statement

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

Despite significant investment in Meta advertising, the business lacks clarity on how effectively advertisements convert into purchases. Fragmented campaign data across platforms makes it difficult to attribute conversions accurately and assess ROI. Key contributing factors include varying audience engagement patterns, platform-specific performance differences, and suboptimal budget allocation. Addressing these challenges through structured performance analysis will enable better conversion tracking, improved decision-making, and reduced inefficiencies in future campaigns.


### 3. Objectives

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

- Build a comprehensive performance tracking report for Facebook and Instagram advertising campaigns.  

- Provide clear visibility into campaign reach, engagement, conversions, and budget utilization.  

- Identify the most effective platform based on conversion and ROI metrics.  

- Analyze audience engagement patterns to improve targeting and campaign performance.  

- Track how advertisements convert into purchases to support data-driven optimization.



### 4. Dataset Description

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

The dataset represents Meta advertising campaign data used to analyze performance, engagement, and conversions. It includes four related datasets sourced from **Data Tutorials**: 

* ad events (400,000 rows, 7 columns), 
* campaigns (50 rows, 6 columns), 
* ads (200 rows, 7 columns), and 
* users (9,842 rows, 7 columns).  
<br>

**Dataset Link:** [click here](https://drive.google.com/drive/folders/1zMuw7Am1uUje8unU5wy_MHlRqDmhT-dU)



### 5. Skills and Tools Used

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

#### Skills

- Data Analysis and Interpretation 

- Performance Tracking and Reporting 

- Data Visualization  

- Large-Scale Data Handling  

- Business Insight Generation  

#### Tools
- Power BI  
- DAX  
- Reporting and Dashboarding Tools  



### 6. Methodology

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

This project focuses on analyzing digital advertising performance using multiple related datasets. The methodology outlines the complete process followed—from data ingestion to visualization—using **Power BI and Power Query**, with structured data modeling and business-focused metrics.



#### 6.1 Data Collection & Ingestion

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>
  
The data used in this project was collected from **local storage (drive-based files)** as provided in the project scope. A total of **four datasets** were used for analysis.

##### Data Sources
- Source type: Local files (drive-based datasets)
- File format: Structured tabular files (imported directly into Power BI)
- Tools used: Power BI Desktop, Power Query Editor

##### Ingestion Process
- All four datasets were imported into **Power BI**
- Each dataset was opened in **Power Query** for inspection and transformation
- No external databases or automated pipelines were used



#### 6.2. Data Understanding & Exploration

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>
  
An initial data exploration phase was conducted to understand the structure, relationships, and analytical purpose of each dataset. This step ensured clarity around fact and dimension tables before modeling.

##### Dataset Overview

**Table 1: `ad_events` (Fact Table)**

* Stores event-level logs such as impressions, clicks, shares, comments, and purchases
* Serves as the **primary fact table** since all KPIs are derived from event records
* Used to analyze how and when users interact with ads

**Table 2: `ads`**

* Contains metadata about ad creatives
* Includes campaign association and targeting attributes
* Enables analysis by platform and creative type (e.g., video vs image ads)

**Table 3: `campaigns`**

* Stores campaign-level information such as budget and duration
* Used for calculating cost-related KPIs (CTR, conversion rate, budget analysis)

**Table 4: `users`**

* Contains demographic and interest-based attributes of users
* Supports audience segmentation by age, gender, country, and interests
* Helps evaluate targeting effectiveness

##### Exploration Goals

* Inspect schema and relationships
* Verify data types and key columns
* Identify event distributions and interaction patterns
* Ensure readiness for modeling and KPI calculation





#### 6.3 Data Cleaning & Preprocessing

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

The datasets were largely pre-cleaned; however, essential validation and transformation steps were applied to ensure analytical accuracy.

##### Cleaning & Validation Steps

* Checked for duplicate records
* Verified and corrected data types, especially **date and timestamp fields**
* Ensured consistency across event types and categorical fields

##### Feature Engineering

Two derived columns were added to the `ad_events` table to support time-based analysis:

* **Event Date**: Extracted date from timestamp
* **Event Hour**: Extracted hour from timestamp

```DAX
-- Data transformation / cleaning
Event Date = DATEVALUE(ad_events[timestamp])
Event Hour = HOUR(ad_events[timestamp])
```


#### 6.4 Data Modeling & Analysis
<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>
A structured data model was created using fact and dimension tables, along with calculated tables and measures to support dynamic analysis.

<img src="https://github.com/Nambhidharan18/Meta-Ad-Performance-Analytics-for-ROI-/edit/main/image/Data model.png">


##### Calculated Tables

**1. Dynamic Measure Selector Table**
Used to enable interactive KPI switching across visuals.

```DAX
-- Dynamic measure selection table
Select Dynamic Measures = {
    ("Impressions", NAMEOF('ad_events'[Impressions]), 0),
    ("Engagements", NAMEOF('ad_events'[Engagements]), 1),
    ("Clicks", NAMEOF('ad_events'[Clicks]), 2),
    ("Shares", NAMEOF('ad_events'[Shares]), 3),
    ("Comments", NAMEOF('ad_events'[Comments]), 4),
    ("Purchases", NAMEOF('ad_events'[Purchases]), 5)
}
```

A dynamic title column was added to improve visual context:

```DAX
-- Dynamic title logic
Dynamic Title =
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 0, "Impressions",
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 1, "Engagements",
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 2, "Clicks",
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 3, "Shares",
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 4, "Comments",
IF('Select Dynamic Measures'[Select Dynamic Measures Order] = 5, "Purchases", "Other"
)))))))
```

**2. Calendar Table**
Created to support robust time intelligence analysis.

```DAX
-- Calendar table
Calendar Table = CALENDAR(
    MIN(ad_events[Event Date]),
    MAX(ad_events[Event Date])
)
```

Additional date attributes added:

* Month
* Day Name
* Day Number
* Weekday
* Week Number

##### Measures & KPIs

A total of **19 DAX measures** were created to evaluate performance, including:

* Impressions, Clicks, Shares, Comments, Purchases
* Engagements and Engagement Rate
* CTR (Click Through Rate)
* Conversion Rate and Purchase Rate
* Total Budget and Average Budget per Campaign
* Dynamic titles for age, gender, geography, and time-based analysis

```DAX
# Model training / analysis
# Placeholder for DAX measure logic
```


#### 6.5 Visualization & Reporting
<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

Insights were communicated through an **interactive Power BI dashboard**, designed for clarity, usability, and business decision-making.

##### KPI Metrics Displayed

* Impressions
* Clicks
* Shares
* Comments
* Purchases
* Engagements
* CTR
* Engagement Rate
* Conversion Rate
* Purchase Rate
* Total Budget
* Average Budget per Campaign

##### Visual Analysis Components

**Engagement Breakdown**

* Donut chart by gender
* Bar chart by target age group

**Geographic Distribution**

* Map showing top engaged countries

**Time-Based Trends**

* Stacked bar chart for weekly engagement trends
* Line chart for hourly engagement trends
* Calendar-based views for date-level analysis

**Campaign & Ad Analysis**

* Performance analysis by ad type and creative category
* Dynamic KPI switching for deeper exploration

```plaintext
# Visualization logic
# Power BI visuals and dashboard layout
```



 

### 7. Key Insights & Findings

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

The analysis of the advertising campaigns revealed critical patterns and trends across engagement, audience, format, and timing, highlighting a significant conversion gap in the purchase funnel.

  * **High Engagement, Low Conversion Efficiency:** Campaigns show strong initial performance with high Click-Through Rates (CTR) and Engagement Rates (ER), indicating successful **brand awareness** and **traffic generation**. However, the subsequent **purchase conversion rate** is inefficient, suggesting a bottleneck post-click that requires immediate attention (e.g., poor landing page experience or weak offers).
  * **Target Audience Concentration:** The highest purchase intent and conversion value are observed among **Female users aged 18–30**, particularly in the geographic markets of **India and Brazil**. This audience segment should be prioritized for highly-tailored campaigns.
  * **Superior Ad Format Performance:** **Video and Stories** formats consistently outperform traditional Carousel and Image ads, driving higher engagement and purchase-related actions. This points to the need for a shift in creative strategy toward more immersive and dynamic content.
  * **Optimal Timing for Conversions:** Ad impressions scheduled during the **afternoon and evening** hours demonstrate a higher likelihood of resulting in a purchase. Optimizing ad delivery to these specific time slots will maximize return on ad spend (ROAS).
  * **Platform Specificity:** Analysis showed that **Facebook** currently delivers a higher volume of purchases compared to Instagram, despite the potential for high engagement on the latter. This warrants a differential strategy for budget allocation and campaign focus across platforms.



### 8. Business Recommendations

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

Based on the conversion gap identified, these recommendations focus on optimizing the ad budget, refining the target strategy, and improving post-click user experience to achieve the target goal of **Growth** and **Efficiency**.

| Recommendation | Linked Insight | Business Impact (Goal: Growth/Efficiency) |
| :--- | :--- | :--- |
| **1. Implement a Full-Funnel Conversion Strategy** | High Engagement, Low Conversion Efficiency | **Efficiency:** Directly address the post-click bottleneck. **Action:** Immediately audit and A/B test landing page designs, streamline checkout flows, and introduce compelling, time-bound offers to significantly lift the purchase conversion rate. |
| **2. Reallocate Budget to High-Value Segments and Formats** | Target Audience Concentration & Superior Ad Format Performance | **Efficiency & Growth:** Maximize ROAS. **Action:** Increase ad spend concentration (e.g., by 30-40%) toward the **Female 18–30** demographic in **India & Brazil**, utilizing **Video and Stories** formats. Scale back budget on underperforming segments/formats. |
| **3. Enhance Retargeting Campaigns** | High Engagement, Low Conversion Efficiency | **Growth:** Capture lost sales. **Action:** Develop sophisticated retargeting campaigns segmented by user behavior (e.g., cart abandoners, high-scroll engagement) to bring interested users back to the optimized landing pages with personalized incentives. |
| **4. Optimize Ad Scheduling** | Optimal Timing for Conversions | **Efficiency:** Reduce wasted spend. **Action:** Shift the majority of the campaign budget to run specifically during the **afternoon and evening** periods identified as high-conversion slots, adjusting geo-specific time zones accordingly. |
| **5. Differentiate Platform Strategy** | Platform Specificity | **Efficiency & Growth:** Maximize platform strengths. **Action:** Maintain Facebook as the primary platform for high-intent purchase conversions, while using Instagram for upper-funnel activities like brand awareness and engagement to feed the retargeting pool. |



### 9. Conclusion

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

This project successfully analyzed the performance of cross-platform digital advertising campaigns, addressing the initial challenge of identifying the most effective spend and conversion drivers. The analysis highlighted a critical conversion bottleneck in the purchase funnel, despite strong upper-funnel engagement. Key outcomes included identifying the most profitable audience segment (Female, 18–30, India/Brazil), establishing optimal ad formats (Video/Stories), and determining platform-specific conversion strengths. The insights provide an actionable roadmap to immediately optimize budget allocation and focus conversion efforts on improving post-click experience, ultimately delivering a clear strategy for maximizing campaign ROI and driving sustainable business growth.



### 10. Future Enhancements

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

To build on the initial analysis and further optimize campaign performance and scalability, the following enhancements are recommended:

  * **Longitudinal Performance Analysis:** Collect an additional 6–12 months of data to perform a year-over-year (YoY) performance analysis, identifying seasonal trends and long-term changes in audience behavior and platform effectiveness.
  * **Creative A/B Testing Matrix:** Implement a structured A/B testing framework to systematically test creative variables (e.g., calls-to-action, tone, messaging) within the top-performing Video and Stories formats.
  * **Landing Page Heatmap and User Flow Analysis:** Integrate specialized tools (e.g., Hotjar) to visualize user interaction on high-traffic landing pages, identifying precise drop-off points and friction areas for micro-level optimization.
  * **Lifetime Value (LTV) Integration:** Integrate Customer Lifetime Value data into the analysis to shift optimization efforts from immediate purchase rate to maximizing the long-term value generated by different ad campaigns and audience segments.



### 11. Folder Structure
<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" target="_blank">
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

A simple, industry-standard structure suitable for a data analysis project using Power BI.

```
[Project Name]/
├── Dataset/
│   └── ad_events.csv
│   └── ads.csv
│   └── users.csv
│   └── campaigns.csv
├── Image/
│   └── pngimg.com - meta_PNG5.png
│   └── Facebook_Logo_2023.png
│   └── pngimg.com - meta_PNG7.png
│   └── images.png
│   └── Google_Ads_logo.svg.png
│   └── Instagram_icon.png
│   └── Threads_(app).png
│   └── whatsapp.png
├── Dashboard/
│   └── Meta Ad Dashboard.pbix
└── README.md
```



### 12. References

<p align="left">
  <a href= "https://www.linkedin.com/in/nambhidharan-s/" targer='_black'>
    <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width= 1200>
  </a>
</p>

The following resources and tools were utilized for data cleaning, analysis, visualization, and project development.

  * **Primary Tool:** Microsoft Power BI
  * **Data Source:** Internal advertising campaign dataset (e.g., Facebook Ads Manager, Google Analytics export)
  * **Learning Resources/Tutorials:**
      * YouTube Tutorial: *[Tutorial Name - If known]* (e.g., Power BI Data Transformation) - [https://youtu.be/8fe9wENTdtU?si=\_o4eLQt0zgNXPQdB](https://youtu.be/8fe9wENTdtU?si=_o4eLQt0zgNXPQdB)
  * **Project Data/Assets:**
      * Shared Data Repository: [Link to Google Drive Folder] - [https://drive.google.com/drive/folders/1zMuw7Am1uUje8unU5wy\_MHlRqDmhT-dU](https://drive.google.com/drive/folders/1zMuw7Am1uUje8unU5wy_MHlRqDmhT-dU)








