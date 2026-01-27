 **Milestone 2 – Hotel Analytics Dashboard - Power BI Visualization**

📌 Project Overview
This project presents an **interactive Hotel Analytics Dashboard** built using **Power BI**. The dashboard provides insights into hotel bookings, revenue, occupancy, guest behavior, and seasonal trends. It helps stakeholders understand performance across booking channels, guest types, countries, and seasons for better data‑driven decision‑making.

🎯 Objectives
* Analyze **booking sources** and their revenue contribution
* Monitor **occupancy and revenue KPIs**
* Understand **guest demographics and behavior**
* Identify **seasonal trends** in bookings and revenue
* Enable interactive filtering for deeper insights

📊 Dashboards Included

🎛️ Filters & Slicers

The dashboard includes interactive slicers for:

* Season
* Booking Channel (Direct / OTA)
* Hotel Branch (Airport / City / Resort)
* Room Category (Deluxe / Standard)
* Stay Type
* Guest Country
* Customer Type

 **Booking Source Comparison**

Purpose: Compare performance across booking channels.

-> Key Visuals:

* Total Revenue by Booking Channel (Direct vs OTA)
* Total Bookings by Booking Channel
* Booking Duration & Total Bookings by Season
* New Bookings Trend by Season
* KPI Card: Total Bookings

-> Insights Provided:

* Revenue contribution of Direct vs OTA channels
* Seasonal impact on booking duration and volume

**Guest Analysis**

 Purpose: Analyze guest demographics and behavior.

-> Key Visuals:

* Bookings by Guest Country (Map & Bar Chart)
* Guest Type Distribution (Leisure vs Business)
* Customer Type Analysis:

  * First‑Time Guests
  * Loyal Guests
  * High Spenders
* Average Nights Stayed
* Total Customers & Bookings

**Occupancy & Hotel Revenue Metrics**

Purpose: Track overall hotel performance.

-> Key KPIs:

* Average ADR (Average Daily Rate)
* RevPAR (Revenue per Available Room)
* Total Revenue
* Occupancy Percentage
* Total Bookings

-> Additional Visuals:

* Bookings by Stay Type (Medium / Long)
* Revenue & Bookings by Booking Channel
* Monthly & Seasonal Booking Trends
* Revenue by Guest Country
* Customer Category vs Guest Type Analysis

**DAX Measures & Calculated Columns**

-> These DAX measures and calculated columns are actively used in the dashboard visuals, KPI cards, charts, and slicers.

The following DAX expressions were used to create key metrics and classifications in the dashboard:

1️⃣ Customer Type (Calculated Column)
Customers Type = 
SWITCH(
    Fact_Bookings[Customer_category],
    1, "First-Time Guest",
    2, "Loyal Guest",
    3, "High Spender",
    "Unknown"
)

Purpose: Categorizes customers into meaningful business segments for guest analysis.

2️⃣ Occupancy Percentage (Measure)
Occupancy % = 
DIVIDE(
    SUM(Fact_Bookings[Reserved_Rooms]),
    SUM(Fact_Bookings[Available_Rooms]),
    0
)

Purpose: Calculates hotel occupancy rate based on reserved and available rooms.

3️⃣ Total Bookings (Measure)
Total Bookings = 
COUNTROWS(Fact_Bookings)

Purpose: Returns the total number of bookings for KPI cards and trend analysis.

 📌 Conclusion
This Hotel Analytics Dashboard provides a comprehensive view of hotel operations, enabling management to track performance, identify trends, and make informed strategic decisions using interactive and visually rich reports.

