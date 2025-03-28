# 🎬 Movie Ticket Booking Analysis

- **Access the dataset and project files:** [Google Drive](https://drive.google.com/drive/folders/1S6RWq4wGdKQW-XDwSnWStFUlUEk8ta2H?usp=sharing)
- **View the code:** [Code.ipynb](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/b2707172f1e9741f1fd2450fc9ebded8a8de0543/%5BPYTHON%5D_PROJECT_MOVIES_TICKETS_Thuy_Linh_Nguyen%20(2).ipynb) 
- **View the full code and outputs:** [Google Colab](https://colab.research.google.com/drive/1H5gk1P-8wfCGGwXF77L5GNXdW7BOCS39?usp=sharing)
- **View the Insights & Recommendations:** [PDF](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/3caa83da0738acd4d44049a0b8d2285d069c6dea/%5B4%5D%20Insights%20%26%20Recommendations.png)

## 📌 Objective
This project analyzes **Online Ticket Booking Behavior** over **4 years** (2019–2023). It will:
+ Identify customer segments and purchasing trends
+ Analyze factors influencing booking decisions
+ Assess customer experience with feedback
#### **The insights will help the companies understand their customers' preferences, optimize marketing efforts, and enhance business strategies**
#### ❓ *Key Question: What are the key characteristics of customer behavior, and what actions should we take to boost sales and improve product quality?*

---

## 📂 Data
The [Dataset](https://drive.google.com/drive/folders/1S6RWq4wGdKQW-XDwSnWStFUlUEk8ta2H?usp=sharing) contains transaction records from a movie ticket booking application (2019–2021) and consists of five tables [Database Scheme](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/b461a3ce5fc705b45e987f3c0965343c48033cb9/%5B1%5D%20Database%20Scheme%20.png)

- `ticket_history.csv` – Movie ticket transactions (customer info, cinema name, movie title, showtime, ticket price, discounts, payment method, etc)
- `status_detail.csv` – Transaction status details
- `device_detail.csv` – Device details used for booking
- `customer.csv` – Customer information and demographics
- `campaign.csv` – Promotional campaign details

---

## ⚡ Approach
Before the analysis processing, I have built [Logical tree](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/b461a3ce5fc705b45e987f3c0965343c48033cb9/%5B2%5D%20Outline%20of%20Logical%20Tree.png) to outline key areas of exploration  
The analysis was conducted in **Google Colab using Python**, utilizing:
- `pandas` for data processing
- `matplotlib & seaborn` for visualization

### **📌 Data Preparation:** 
- Loading, cleaning, and merging tables

 ### **📌Exploratory Analysis:**
- Checked dataset structure (`info()`) and unique values
- Analyzed missing values using **a custom function to calculate the percentage of null values per column**

### **📌 Visualizations:** 
- Line charts, Pie charts, Bar charts, 100% stacked area charts (via pivot tables)

### **📌 Statistical Insights:** 
- Distribution analysis using histograms to detect outliers and identify trends

### **📌 Segmentation:**
- Created **dimension tables** to segment data by **age group, promotion usage, payment method, model type**, etc
- Built a **TIME dimension table** to ensure all **YearMonth** values are present for complete time series analysis

### **📌 Customer Retention:**
- Conducted **Cohort Analysis** to track user retention in 2019 & 2022
- Used **Seaborn heatmaps** to visualize retention trends across different cohorts

Finally, a [mind map](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/b461a3ce5fc705b45e987f3c0965343c48033cb9/%5B4%5D%20Insights%20%26%20Recommendations.png) summarizes key insights, findings, and recommendations

---

## 📊 Results

- [View the results with the charts](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/2ca66b24a9cf6d2fb62b88f294b063a8042ebf96/%5B3%5D%20Insights%20%26%20Charts.png)
- [View the insights and personal recommendations](https://github.com/ngthuylinh3003/Movie_Ticket_Python/blob/2ca66b24a9cf6d2fb62b88f294b063a8042ebf96/%5B4%5D%20Insights%20%26%20Recommendations.png)

#### **Customer Portraits**:
- **Gen Y/Millennials (29-44 years old)** account for **60%** of customers, followed by **Gen Z (36%)**
- The distribution of the **55+ age group** is unusual
- **Gender distribution** is **balanced**, with **11% unidentified** customers

#### **Trends (Peak Seasons):**
- **Monthly:** Two peak seasons: **May–July (summer) & Oct–Dec (year-end)**
- **Weekly:** Higher activity on **weekends**
- **Hourly:** Peak hours are **11 AM–1 PM** and **6 PM–8 PM**
=> *Marketing focus should align with these timeframes*

#### **Payment Behavior:**
- **89%** of customers book tickets via the **app (iOS/Android/Others)**
- **77%** use **in-app payment ('money in app')**

#### **The no of Tickets:**
- Most customers buy only a few tickets (73.58% for 1 ticket and 13.4% for 2-3 tickets)
- But a few top buyers (5 customers) **purchase a lot** (>100 tickets) -> However, their purchases are spread out over time, so there is nothing unusual
  
#### **Promotion Usage:**
- **~58%** joined **at least one promotion**; among them, **89%** used a promotion **only once**
- The most popular promotion is **‘direct discount’ (87%)**

#### **Retention Rate (2019 vs. 2022):**
- **Minimal difference** between both years
- **1-month retention is very low**, averaging **only 3% in 2022**, despite **63% of customers** using promotions

#### **Success Rate:**
- Overall success rate is good ~ **80-90%**
- **‘Money in app’ payment method** has the highest success rate (**97%**)
- **10%** of customers face payment errors, mostly due to **bank-related issues (third-party ‘bank account’ payments)**

---

## 🎯 Personal Recommendations

### **Increase Sales:**
- **Target the 19-25 age group** for new customers
- **Leverage peak times/seasons** for marketing efforts
- **Implement cross-selling strategies** and enhance services to retain customers post-promotion

### **Improve Product:**
- **Enhance the user interface** for a better booking experience
- **Encourage in-app payments** to increase transaction success rates
- **Partner with third-party banks** to minimize transaction errors and payment failures

---
📌 This analysis reflects my personal perspective and approach. **I’d love to hear your feedback and suggestions!**




