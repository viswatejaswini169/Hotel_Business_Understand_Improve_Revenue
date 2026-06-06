#🏨 HotelRevAI: AI-Driven Revenue Analysis for Hotels

#📌 Project Overview
This project leverages data modeling, advanced analytics, and AI-powered forecasting to analyze hotel booking patterns, guest behavior, upselling opportunities, and revenue performance. Interactive dashboards and visual reports translate complex data into actionable business insights for the hospitality industry.

#📂 Modules

#1. 🗄️ Data Modeling

Standardized data types and handled data quality issues
Built normalized tables: Room, Customer, Date, Hotel connected via Star Schema
Derived key columns: booking_id, customer_id, arrival_date using merge queries

#2. 📈 Occupancy & Revenue Analysis

Tracked RevPAR, ADR, and daily occupancy across seasonal, weekly, and monthly trends
Insight: Peak season is August–September; high occupancy generally drives higher RevPAR

#3. 👥 Guest Analysis

Analyzed bookings by stay type, customer type, and country using bar and pie charts
Insight: Business guests dominate bookings; most guests are from Portugal

#4. 🔮 Forecasting & Cancellation

Used Facebook Prophet model for month-wise forecasting of bookings, revenue, and cancellations
Insight: monsoon season and OTA platforms show the highest cancellation rates

#5. 💰 Upselling & Revenue Optimization

Assigned upsell scores per booking; segmented into High, Medium, and Low spender tiers
Insight: Total weekend stays and business class lead in revenue contribution

#🛠️ Tools & Technologies

Power BI
Power Query
Python (Prophet)
Star Schema
DAX
