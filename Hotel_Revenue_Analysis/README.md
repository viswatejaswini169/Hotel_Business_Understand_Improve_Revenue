# Hotel Business Understand Improve Revenue

# Data Modelling
1) changed data types 
2) corrected the errors by replacing them with null if the column is integer or a number type
3) made room, customer, date, hotel tables
4) connect tables through a star schema(one to many relation)
5) made columns such as booking id using index column
6) through merge queries connected the tables and made customer id column
7) Used  merging to make arrival date column
8) replaced the values in some columns to make it fit for using data
9) blanked rows were removed .

# Occupancy and Revenue 
* data is classified as seasonal,daily,weekly etc.

Approach :
1) calculated trend paramter using the columns arrival week start,arrival month start and arrival data, 
2) Made measures such as revpar, revenue, room sold, room available
3) X axis -  used trend and on Y-axis used sum of adr, revpar,  average of revenue etc

## Columns Used
1) Avg daily occupancy
2) RevPar
3) customer id
4) sum of adr
5) average of revenue

## Observations
1) We can mesasure sum of adr, Revpar, Avg daily occupancy using weeks,months and arrival dates.
2) When avg daily occupancy is high then revpar generated is also high but in some cases its the opposite
3) The peak season for customers to come is august and september


# Guest Analysis
Approach :
1) Used total bookings on Y axis and stay type on X axis to know which stay has most number of bookings
2) Measures for total booking were calculated by counting the number of booking ids
3) used pie charts for distinguishing the total bookings through spend type
4) used clustered column chart for looking the most contributing category 


## Columns Used
1) total bookings
2) stay type
3) customer type
4) country
5) average of total nightsav

## Observations
1)  Business guests have the most number of bookings.
2)  Most bookings are done for standard stay type.
3)  Maximum bookings are from portugal.
4)  We have total 880 customers.

# Forecasting and Cancellation
Approach :
1)  create  a monthwise booking table and export the data in csv format
2)  the code uses prophet model 
3)  Used Prophet to make the model and used methods such as predict and fit to get the result.
4)  made a forecast function which is used for every column in the input table monthwise booking table.


## Columns Used
1) Sum of adr forecast
2) sum of total bookings forecast
3) sum of revenue forecast
4) sum of cancellation % forecast
5) actuall bookings last 12 months
6) forecast growth



## Observations
1) the forecasted cancellation rate is same across three years 2015,2016,2017
2) total forecasted bookings are 65.02K 
3) Forecasted total bookings monthwise are approximately same as the given total bookings
4) most number of cancelled bookings are from portugal
5) Season monsoon has the most cancelled bookings
6) Through OTA platform most bookings are cancelled

As we are getting positive results
1) use this data for predicting the results for future
2) focus on direct booking as its graph is suddenly increasing and decreasing in total bookings. 



# Upselling and Revenue
Approach :
1)  used if condition to get upsell score based on stay and comparison for adr
2) the upsell category were made through upsell score
3) used pie charts and donut charts to look at the contribution from upsell category
4) divide(high upsell booking / total bookings) is used for getting high upsell percentage.

## Business Implications
1) focus on increasing the high upsell number
2) Focus on high spenders and medium spenders

## Columns Used
1) Upsell Category
2) % High Upsell
3) High Upselling bookings
4) Upsell score

## Observations
1) spend type is differentiated into high spenders, low spenders and medium spenders
2) total revenue generated is 32.88M
3) the high upsell bookings are 3K 
4) the weekend stay is making the most revenue and also business class is the leading class


Note - **Slicers such as for hotel type , month, booking channel, room_id are common across all reports. 
