# 📊 Social Media Campaign Performance Dashboard (Power BI)

## 📖 Overview
This project analyzes global social media advertising performance using Power BI.  
It focuses on understanding user behavior, campaign effectiveness, and ad performance using datasets like **users, ads, ad_events, and campaigns**.

---

## 🎯 Objectives
- Analyze user activity by **day of week and time of day**
- Measure campaign performance using **CTR, Engagement, and Conversions**
- Identify **high-performing audience segments**
- Compare ad effectiveness across **platforms and ad formats**
- Generate insights for **data-driven marketing decisions**

---

## 📂 Datasets Used
- **users.csv** → User demographics (age, gender, country)
- **ads.csv** → Ad details (platform, ad type)
- **ad_events.csv** → Event-level data (impressions, clicks, conversions)
- **campaigns.csv** → Campaign details

---

## 🔗 Data Model
Relationships created:
- `ad_events[userid] → users[userid]`
- `ad_events[adid] → ads[adid]`
- `ads[campaignid] → campaigns[campaignid]`

---

## 📊 Visualizations

### 📅 User Activity
- Bar Chart → Number of users by **Day of Week**
- Pie Chart → Users by **Time of Day**

---

## ⚙️ Event Classification

```DAX
Event Category =
SWITCH(
    TRUE(),
    ad_events[eventtype] = "impression", "Impression",
    ad_events[eventtype] = "click", "Click",
    ad_events[eventtype] = "engagement", "Engagement",
    ad_events[eventtype] = "conversion", "Conversion"
)
