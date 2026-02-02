📊 Forecasting and Cancellation Trends – Power BI Project

📌 Project Overview

This project focuses on analyzing hotel booking data to understand booking trends, cancellations, lead time behavior, and to forecast future monthly bookings.
The solution was implemented using Power BI for data modeling and visualization and Python for forecasting.

The task was completed by:

* Creating a Monthly Bookings table
* Forecasting monthly bookings using Python
* Importing the forecast results into Power BI as a Forecast table
* Creating required DAX measures
* Building interactive Power BI report visuals

🎯 Objectives

Aggregate booking data at a monthly level
Analyze total bookings and cancellations
Calculate average lead time
Forecast future monthly bookings
Identify the peak forecast month
Present insights using Power BI visuals

📂 Data Description
Raw Fact Table :-
The main CSV file acts as the raw fact table and contains:

Sum of Bookings
Sum of Cancellations
Sum of Booking_duration
Month_End_Date (added to support monthly analysis)
Monthly Bookings Table

A Monthly Bookings table was created from the raw fact table to aggregate bookings at the month level.
This table is used for trend analysis and forecasting.

**Forecast Table**

-> Monthly bookings data was exported from Power BI
-> Forecasting was performed using Python

The output contains:

ds – forecast month/date
yhat – predicted bookings
The forecast output was imported back into Power BI as the Forecast table

🧮 DAX Measures Used
🔹 Total Bookings
Total Bookings = 
SUM('data'[Sum of Bookings])

🔹 Total Cancellations
Total Cancellations = 
SUM('data'[Sum of Cancellations])

🔹 Cancellation Rate
Cancellation Rate = 
DIVIDE([Total Cancellations], [Total Bookings], 0)

🔹 Average Lead Time
Avg Lead Time = 
AVERAGE('data'[Sum of Booking_duration])

🔹 Total Forecasted Bookings

Calculates forecasted bookings after the last available actual date.

Total Forecasted Bookings =
CALCULATE(
    SUM(Forecast[yhat]),
    Forecast[ds] > MAX('Date'[arrival_date])
)

🔹 Peak Forecast Month

Identifies the month with the highest forecasted bookings.

Peak Forecast Month =
MAXX(
    VALUES(Forecast[ds]),
    SUM(Forecast[yhat])
)

**Forecasting Using Python**

Monthly bookings data was used as input

Python was used to forecast future bookings

The forecasted output was imported into Power BI

Forecast values are visualized alongside actual bookings

📊 Report Visuals

The Power BI report includes:

KPI cards:

->Total Bookings
->Cancellation Rate
->Average Lead Time
->Total Forecasted Bookings
->Peak Forecast Month

Line charts:

->Actual vs Forecasted Bookings
->Bookings, Forecast, and Occupancy %

Bar charts:

-> Monthly Cancellations and No-Shows
-> Forecasted Bookings by Booking Channel and Season

Slicers for:

->Month
->Season
->Hotel Branch
->Booking Channel


**Conclusion**

This project successfully demonstrates monthly booking analysis, cancellation trends, and demand forecasting using Power BI and Python.
The combination of DAX measures, forecasting, and interactive visuals provides meaningful insights for business decision-making
