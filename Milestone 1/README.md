# Hotel Revenue Analysis

##  Project Overview

This project focuses on analyzing **hotel revenue and booking performance** using **Power BI**. The dashboard provides insights into seasonal revenue trends, guest behavior, booking channels, occupancy, and cancellations. These insights support data-driven decisions to improve revenue management and operational efficiency.

---

## 📂 Dataset Description

**File Name:** `hotel_data.csv`

The dataset includes aggregated hotel-level information related to:

* Total revenue and RevPAR
* Seasons and dates
* Guest type and guest country
* Booking channels
* Check-ins and check-outs
* Occupancy rate and cancellations

The data is aggregated by date and used to derive trends and comparisons across multiple business dimensions.

---

## 🛠 Tools Used

* **Power BI Desktop** – for building interactive dashboards
* **Power Query** – for data cleaning, transformation, and derived columns
* **DAX** – for calculating revenue, RevPAR, occupancy, and aggregation measures

---

## 🧩 Data Modeling

A **Star Schema** model was implemented for efficient analysis and accurate filtering.

### 📊 Fact Table

**Fact_Bookings**

* Stores numerical measures such as revenue, check-ins, check-outs, occupancy rate, cancellations, and RevPAR

### 🗂 Dimension Tables

* **Dim_Date** – Date, season, and time-based attributes
* **Dim_Customer** – Guest type and guest country
* **Dim_Room** – Room-related and occupancy attributes
* **Dim_Hotel** – Logical hotel/branch categorization

### 🔗 Relationships

* One-to-many (1:*) relationships connect all dimension tables to the fact table
* This structure enables accurate slicing and filtering across all visuals

---

## 📈 Key Visualizations

### 1. Revenue by Season

* **Bar Chart**: Sum of Total Revenue by Season
* Shows how revenue varies across Winter, Summer, and Spring

### 2. Revenue Trend by Season

* **Line Chart**: Sum of Revenue by Season
* Highlights the overall decline or growth pattern across seasons

### 3. RevPAR by Guest Type

* **Donut Chart**: Sum of RevPAR by Guest Type (Leisure vs Business)
* Helps understand which guest segment contributes more to room performance

### 4. Check-ins & Check-outs by Booking Channel

* **Donut Chart**: Distribution of Check-ins and Check-outs across booking channels (OTA, Direct, etc.)
* Identifies dominant booking sources

### 5. Revenue by Guest Country

* **Bar Chart**: Sum of Revenue by Guest Country
* Highlights top revenue-contributing countries

### 6. Occupancy Rate and Cancellations Over Time

* **Line Chart**: Occupancy Rate and Cancellations by Date
* Helps analyze demand stability and cancellation behavior over time

## Key Insights

* Winter season generates the highest total revenue
* Leisure guests contribute a higher share of RevPAR compared to business guests
* OTA and Direct channels account for most check-ins and check-outs
* The USA and European countries are major revenue contributors
* Occupancy rate trends are stable, while cancellations show noticeable fluctuations

##  Conclusion

The Hotel Revenue Analysis dashboard provides a comprehensive view of revenue performance, guest behavior, and operational trends. By analyzing seasonality, guest segments, booking channels, and occupancy patterns, hotel management can:

* Optimize pricing and revenue strategies
* Focus on high-performing guest segments and markets
* Improve channel strategy and reduce cancellations
Overall, the project demonstrates how Power BI can be effectively used to transform raw hotel data into meaningful business insights.
