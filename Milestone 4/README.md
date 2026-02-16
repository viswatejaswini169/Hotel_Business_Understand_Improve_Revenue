***Revenue Strategy Insights Dashboard with pricing insights and upsell recommendations***

📌 Project Overview

This project presents a Revenue Strategy Insights Dashboard built using Power BI to analyze hotel booking, pricing tiers, seasonal performance, and revenue optimization opportunities.

The dashboard provides actionable insights into:

**Pricing tier performance**

-> Upsell opportunities

-> Seasonal revenue variations

-> Booking and cancellation patterns

-> Revenue improvement strategies

The objective is to support data-driven pricing and revenue decisions for hotel management.

**Dashboard KPIs**

The dashboard includes the following key performance indicators:

-> Total Revenue: 6M

-> Average Daily Rate (ADR): 14K

-> Occupancy Rate: 28%

-> RevPAR: 10.19K

-> Total Rooms Sold: 985

These KPIs provide a high-level summary of overall revenue performance.

**Pricing Tier Logic Used**

 Room Category Tier Classification

Room categories are grouped into pricing tiers using the following business logic:

          Room Category Tier =
                           SWITCH(
                                  TRUE(),
                                  'Fact Bookings'[Room_category] IN {"Standard","Basic","Classic"}, "Economy",
                                  'Fact Bookings'[Room_category] IN {"Deluxe","Executive"}, "Premium",
                                  'Fact Bookings'[Room_category] IN {"Suite","Presidential","Luxury Suite"}, "Luxury",
                                  "Economy"
                          )

*Tier Explanation

-> Economy Tier

-> Budget-friendly rooms

-> High booking volume

-> Lower ADR

-> Premium Tier

-> Mid-level pricing

-> Balanced revenue contribution

-> Strong upsell potential

-> Luxury Tier

-> High ADR

-> Lower booking count

-> High per-booking revenue

This classification enables comparison of revenue contribution by tier.

📈 Upsell Strategy Identification Approach

Upsell opportunities were identified using:

*Booking Volume vs Revenue Comparison

- Economy has high bookings but lower revenue per booking.

- Premium shows strong revenue potential.

*ADR Analysis

- Higher ADR tiers generate more revenue per guest.

- Guests booking Economy tier can be targeted for Premium upgrades.

*Cancellation Patterns

- High cancellation rates in specific tiers indicate pricing sensitivity.

- Discounted upgrade offers can reduce cancellations.

*Channel Performance

- OTA channels show strong volume.

- Direct channel promotions can encourage premium upgrades.

🎯 Upsell Strategy

- Offer discounted upgrades from Economy → Premium during check-in.

- Bundle Premium rooms with complimentary services.

- Provide loyalty-based upgrades for repeat customers.

🌤 Seasonal Promotion Insights

The dashboard analyzes revenue across:

- Winter

- Summer

- Spring

**Key Observations:**

-> Winter shows highest revenue contribution

-> Summer shows moderate performance

-> Spring shows relatively lower revenue

**Promotion Strategy:**

-> Offer targeted discounts during low seasons (Spring).

-> Increase ADR during peak season (Winter).

-> Launch early-bird summer campaigns.

-> Introduce seasonal packages (family, honeymoon, festival offers).

📊 Revenue Performance Insights

*Revenue by Month

- January and July show high revenue peaks.

- March shows a noticeable dip.

- Seasonal alignment impacts performance.

*Revenue by Room Tier

- Premium tier contributes significantly to revenue.

- Economy has volume advantage.

- Luxury tier boosts overall ADR.

- Revenue by Country

*Major contribution from:

- USA

- Germany

- UK

- Spain

- France

- Italy

This supports geo-targeted marketing campaigns.

🚀 Key Revenue Improvement Recommendations

1️⃣ Optimize Pricing Strategy

- Dynamic pricing during peak season.

- Increase ADR for Premium tier gradually.

- Implement demand-based pricing.

2️⃣ Reduce Cancellations

- Flexible rescheduling options.

- Incentives for non-refundable bookings.

- Offer partial upgrade discounts instead of refunds.

3️⃣ Improve Occupancy Rate

- Bundle packages (room + spa + dining).

- Weekend getaway promotions.

- Corporate booking tie-ups.

4️⃣ Channel Optimization

- Promote direct bookings via website discounts.

- Reduce OTA dependency.

- Loyalty-based booking incentives.

5️⃣ Focus on High-Value Segments

- Target repeat guests.

- Promote long-stay discounts.

- Luxury experience campaigns.

📈 Business Impact of Proposed Strategies

If implemented, these strategies can:

* Increase overall revenue by improving ADR

* Improve occupancy from 28% to higher utilization

* Reduce cancellation losses

* Improve RevPAR

* Enhance customer lifetime value

* Strengthen competitive positioning

📌 Conclusion

The Revenue Strategy Insights Dashboard transforms booking data into strategic decision-making insights.

By combining pricing tier logic, seasonal analysis, upsell identification, and revenue KPIs, the dashboard enables management to:

*Optimize pricing

*Improve occupancy

*Increase profitability

*Strengthen long-term revenue growth
