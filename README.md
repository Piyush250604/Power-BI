# 📊 Campaign Performance Analysis (Power BI Project)

![Power BI](https://img.shields.io/badge/Tool-Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Domain-Marketing_Analytics-blue?style=for-the-badge)
![Project Type](https://img.shields.io/badge/Type-Analytics_Project-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Overview
This project focuses on analyzing digital advertising campaign performance using **Power BI**.  
The analysis is based on multiple datasets including users, ads, ad events, and campaigns.

The objective is to build an interactive dashboard and extract meaningful insights related to campaign effectiveness, user behavior, and ad performance.

---

## 📂 Datasets
The project uses the following datasets:

- 👤 `users.csv` – User demographics (age group, gender, country)  
- 📢 `ads.csv` – Ad details (platform, ad type)  
- 📊 `ad_events.csv` – User interactions (impressions, clicks, engagements, conversions)  
- 🎯 `campaigns.csv` – Campaign-level information  

---

## 🎯 Project Objectives

✔️ Visualize user activity by **day of week** and **time of day**  
✔️ Design a **data model** connecting all datasets  
✔️ Classify ad events into meaningful categories  
✔️ Create key **marketing performance metrics (KPIs)**  
✔️ Analyze **time-based user behavior**  
✔️ Perform **audience segmentation analysis**  
✔️ Evaluate **ad performance across platforms & formats**  
✔️ Build an **interactive Power BI dashboard**  

---

## 🔗 Data Model Design

Relationships created:

- `ad_events.user_id` → `users.user_id`  
- `ad_events.ad_id` → `ads.ad_id`  
- `ads.campaign_id` → `campaigns.campaign_id`  

---

## ⚙️ Metrics & Calculations

### 📌 Event Classification
Events categorized into:
- Impression  
- Click  
- Engagement  
- Conversion  

### 📊 DAX Measures
```DAX
Total Impressions = COUNTROWS(FILTER(ad_events, ad_events[event_type] = "Impression"))

Total Clicks = COUNTROWS(FILTER(ad_events, ad_events[event_type] = "Click"))

CTR = DIVIDE([Total Clicks], [Total Impressions])

Total Engagements = COUNTROWS(FILTER(ad_events, ad_events[event_type] = "Engagement"))

Total Conversions = COUNTROWS(FILTER(ad_events, ad_events[event_type] = "Conversion"))
```
## 📊 Data Visualization

### 📈 Charts Created
- Bar Chart: Users by **Day of Week**  
- Pie Chart: Users by **Time of Day**  

---

## ⏱️ Time-Based Analysis

- Impressions & Clicks by **Day of Week**  
- CTR by **Time of Day** (Morning, Afternoon, Evening, Night)  

---

## 👥 Audience Segmentation

### Segments Created Using:
- Age Group  
- Gender  
- Country  

### 📊 Matrix Analysis
- Impressions  
- Clicks  
- CTR  
- Conversions  

---

## 📢 Ad Performance Analysis

### Compared Across:
- Platforms: Facebook vs Instagram  
- Ad Types: Video, Image, Carousel, Stories  

### 📊 Metrics
- Impressions  
- Clicks  
- CTR  
- Engagement Rate  
- Conversion Rate  

---

## 📊 Dashboard Features

### ✅ 4 KPI Cards:
- Total Impressions  
- Total Clicks  
- CTR  
- Total Conversions  

### 📈 2 Charts:
- User Activity Trends  
- Campaign Performance  

### 🎛️ Dynamic Filter:
- Platform / Campaign / Segment  

---

## 🛠️ Tools & Skills Used

- 📊 Power BI  
- 📌 Data Modeling  
- 🔢 DAX (Data Analysis Expressions)  
- 🔄 Power Query  
- 📈 Data Visualization  

---

## 📁 Project Files

| File Name                 | Description                     |
|--------------------------|---------------------------------|
| Campaign Dashboard.pbix  | Power BI Dashboard File         |
| datasets/                | Raw datasets used in analysis   |

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/Piyush250604/Power-BI.git
   ```
2. Open `.pbix` file in Power BI Desktop  
3. Explore dashboard and insights  

---

## 💡 Learning Outcomes

- Built interactive dashboards in Power BI  
- Developed strong understanding of DAX  
- Learned data modeling techniques  
- Performed marketing campaign analysis  
- Improved data visualization skills  

---

## 🔗 Connect With Me

- 💼 LinkedIn: [Piyush Bhardwaj](https://www.linkedin.com/in/piyush-bhardwaj25604/)
- 📧 Email: [Mail Piyush](piyush2004bhardwaj@gmail.com)  
