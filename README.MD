# 🏨 Hospitality Revenue & Performance Dashboard — Power BI

![Dashboard Home](/Image/Image.png)

## 📌 Introduction

This **Hospitality Revenue & Performance Dashboard** was built in **Power BI** to analyze hotel booking performance and provide actionable insights into **revenue, occupancy, room utilization, booking platforms, and property performance**.

The project is uses a real-world hospitality dataset containing hotel properties, room categories, booking information, revenue, booking platforms, ratings, and daily capacity.

The dashboard brings all of this information into a single interactive interface, allowing users to analyze hotel performance across **cities, property categories, room classes, and time periods**.

---

## 🎯 Project Objective

The primary objective of this project is to transform raw hotel booking data into an interactive business intelligence dashboard that helps answer questions such as:

* How much revenue is being generated?
* What is the overall hotel occupancy?
* Which properties are performing well?
* How are **ADR** and **RevPAR** changing over time?
* What percentage of bookings are being realized?
* Which booking platforms generate the most bookings?
* How does performance differ between **Luxury** and **Business** hotels?
* How do different room categories perform?
* How does hotel performance vary between weekdays and weekends?

---

## 📊 Dataset

The project uses multiple CSV files representing a simple hospitality data model.

### Dimension Tables

**`dim_date.csv`**

* Date
* Month & Year
* Week Number
* Day Type

**`dim_hotels.csv`**

* Property ID
* Property Name
* Hotel Category
* City

**`dim_rooms.csv`**

* Room ID
* Room Class

### Fact Tables

**`fact_bookings.csv`**

* Booking ID
* Property ID
* Booking Date
* Check-in Date
* Checkout Date
* Number of Guests
* Room Category
* Booking Platform
* Ratings
* Booking Status
* Revenue Generated
* Revenue Realized

**`fact_aggregated_bookings.csv`**

* Property ID
* Check-in Date
* Room Category
* Successful Bookings
* Capacity

---

## 🛠️ Skills & Power BI Features Showcased

### ⚙️ Data Transformation with Power Query

Used **Power Query** to prepare the raw datasets for analysis, including:

* Data cleaning
* Data type transformation
* Handling missing values
* Preparing dimension and fact tables
* Creating a structured analytical dataset

### 🧮 DAX Measures

Created business-oriented measures to calculate important hospitality KPIs, including:

* Revenue
* Total Bookings
* RevPAR
* ADR
* Occupancy %
* DSRN
* DBRN
* DURN
* Realisation %
* Cancellation %
* Average Rating
* Week-over-Week performance changes

### 📈 Data Visualization

The dashboard uses multiple Power BI visualizations, including:

* KPI Cards
* Donut Chart
* Line Chart
* Combo Chart
* Tables
* Conditional Formatting
* Slicers
* Interactive filters

### 🖱️ Interactive Dashboard

Users can dynamically filter the dashboard using:

* **City**
* **Room Class**
* **Hotel Category**
* **Month**
* **Week**

This allows users to move from a high-level business view to more detailed property and operational analysis.

---

# 📊 Key Hospitality KPIs

The dashboard focuses on several important hotel performance metrics.

### 💰 Revenue

Total realized revenue generated from hotel bookings.

### 🏨 Occupancy %

Measures the percentage of available room capacity that was successfully booked.

### 💵 ADR — Average Daily Rate

Measures the average revenue earned per occupied room.

### 📈 RevPAR — Revenue per Available Room

Measures revenue performance across the total available room capacity.

### 👥 DSRN — Daily Sellable Room Nights

Measures the number of rooms available for sale over the selected period.

### 🛏️ DBRN — Daily Booked Room Nights

Measures the number of rooms booked over the selected period.

### 🌙 DURN — Daily Utilized Room Nights

Measures the number of rooms actually utilized by guests.

### ✅ Realisation %

Measures the percentage of bookings that were successfully realized compared with total bookings.

### ❌ Cancellation %

Shows the proportion of bookings that were cancelled.

### ⭐ Average Rating

Shows the average rating given by guests.

---

# 🖥️ Dashboard Overview

## Page 1: Hospitality Performance Overview

![Dashboard Page 1](images/Project_page1.png)

The main dashboard provides a high-level overview of hotel performance.

### KPI Section

The dashboard displays key metrics such as:

* **Revenue**
* **RevPAR**
* **DSRN**
* **Occupancy %**
* **ADR**
* **Realisation %**

These KPIs provide a quick snapshot of the overall business performance.

### Hotel Category Analysis

A donut chart compares revenue performance between:

* Luxury Hotels
* Business Hotels

This allows users to understand how different hotel categories contribute to overall revenue.

### Trend Analysis

The **Trend by Key Metrics** visualization tracks important performance indicators over time, including:

* RevPAR
* ADR
* Occupancy %

This helps identify changes in hotel performance across different weeks.

### Booking Platform Analysis

The dashboard also compares booking platforms using metrics such as:

* Realisation %
* ADR

This provides insight into how different booking channels perform.

### Property-Level Analysis

The **Property by Key Metrics** table provides a detailed comparison of individual hotel properties using metrics such as:

* Revenue
* Total Bookings
* RevPAR
* Occupancy %
* ADR
* DSRN
* DBRN
* DURN
* Realisation %
* Cancellation %
* Average Rating

Users can therefore move from an overall business view to individual property performance.

---

# 📁 Data Model

The project follows a dimensional data-model approach with separate **dimension** and **fact** tables.

### Dimension Tables

```text
dim_date
    │
    ├── Date
    ├── Month
    ├── Week
    └── Day Type

dim_hotels
    │
    ├── Property ID
    ├── Property Name
    ├── Category
    └── City

dim_rooms
    │
    ├── Room ID
    └── Room Class
```

### Fact Tables

```text
fact_bookings
    │
    ├── Booking information
    ├── Customer information
    ├── Booking platform
    ├── Booking status
    └── Revenue

fact_aggregated_bookings
    │
    ├── Successful bookings
    └── Room capacity
```

This structure makes it easier to build reusable DAX measures and analyze hotel performance across different dimensions.

---

# 📌 Dataset Overview

The dataset contains approximately:

* **134K+ booking records**
* **25 hotel properties**
* **4 cities**
* **4 room categories**
* **7 booking platforms**
* **2 hotel categories**
* **92 days of hotel performance data**

The hotel properties are distributed across:

* Delhi
* Mumbai
* Hyderabad
* Bangalore

The two major hotel categories are:

* **Luxury**
* **Business**

---

# 🔍 Business Insights Enabled by the Dashboard

The dashboard can be used to investigate:

### Property Performance

Compare individual hotel properties based on revenue, bookings, occupancy, ADR, and RevPAR.

### Revenue Performance

Understand how revenue changes over time and how different hotel categories contribute to total revenue.

### Occupancy Analysis

Identify periods and properties with higher or lower room utilization.

### Booking Channel Performance

Compare direct and third-party booking platforms based on realization and ADR.

### Room Performance

Analyze how different room classes contribute to hotel performance.

### Operational Performance

Use DSRN, DBRN, DURN, occupancy, and realization metrics to understand room availability and utilization.

---

# 🧰 Tools & Technologies

* **Power BI Desktop**
* **Power Query**
* **DAX**
* **Microsoft Excel / CSV**
* **Data Modeling**
* **Data Visualization**
* **Business Intelligence**

---

# 📂 Project Structure

```text
Hospitality-Revenue-Performance-Dashboard/
│
├── HospitalityDomain.pbix
│
├── Data/
│   ├── dim_date.csv
│   ├── dim_hotels.csv
│   ├── dim_rooms.csv
│   ├── fact_aggregated_bookings.csv
│   └── fact_bookings.csv
│
├── images/
│   └── Project_page1.png
│
└── README.md
```

---

# 🎓 What I Learned

Through this project, I strengthened my understanding of:

* Building a Power BI data model
* Working with fact and dimension tables
* Data cleaning using Power Query
* Creating calculated measures using DAX
* Designing hospitality-specific KPIs
* Creating interactive dashboards
* Using conditional formatting
* Analyzing time-based trends
* Comparing property-level performance
* Turning raw business data into actionable insights

---

# 🚀 Conclusion

This project demonstrates how **Power BI can transform raw hospitality booking data into an interactive business intelligence solution**.

By combining **Power Query, data modeling, DAX, and interactive visualizations**, the dashboard provides a comprehensive view of hotel performance across revenue, occupancy, bookings, room utilization, booking platforms, and individual properties.

The project also demonstrates how business-specific KPIs such as **RevPAR, ADR, Occupancy %, Realisation %, DSRN, DBRN, and DURN** can be used to evaluate hospitality performance and support data-driven decision-making.

---

## 👨‍💻 Project

**Hospitality Revenue & Performance Dashboard**

**Built with:** Power BI | Power Query | DAX | Data Modeling | Data Visualization
