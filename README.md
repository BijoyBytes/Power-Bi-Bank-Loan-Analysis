# Financial Analysis – Bank Loan Performance – Power BI

## Project Overview

**Project Title:** Revenue Insights in Hospitality Domain  
**Level:** Intermediate  
**Tool:** Microsoft Power BI  

This project showcases the use of Power BI to analyze and visualize key revenue metrics in the hospitality sector. It provides interactive dashboards to help stakeholders understand trends, track performance, and make data-driven decisions.

![Library_project](https://github.com/BijoyBytes/Power-Bi-Hospitality-Analysis/blob/main/wmremove-transformed.jpeg)




##  Objectives

1. Develop interactive dashboards to explore revenue and occupancy trends.
2. Enable dynamic filtering by time period, property, and customer segment.
3. Highlight key performance indicators (KPIs) such as ADR, RevPAR, and Occupancy Rate.
4. Identify revenue drivers and underperforming segments.
5. Share insights with management through an accessible Power BI report.


##  Project Structure

### 1. Data Sources & Preparation
- Imported booking and property data.
- Applied Power Query transformations:
  - Removed duplicates.
  - Cleaned date formats.
  - Merged lookup tables.
- Created calculated columns and measures.

### 2. Data Model
- Defined relationships between fact and dimension tables.
  - **Dimension Table**: dim_date, dim_hotels, dim_rooms
  - **Fact Table**: fact_bookings, fact_aggregated_bookings

  ![Library_project](https://github.com/BijoyBytes/Power-Bi-Hospitality-Analysis/blob/main/Data_Modiling_Hospitality.png)

- Built DAX measures to compute KPIs:
  ```dax

  • ADR (Average Daily Rate) - Total Rooms Revenue/ No. of Rooms Sold
  
  • DSRN (Daily Sellable Room Nights) = Total Rooms Available to Sell/ No. of Days
  
  • DURN (Daily Utilized Room Nights) = Total Checked out/ No. of Days
  
  • DBRN (Daily Booked Room Nights) = Total Bookings/No. of Days
  
  • Occupancy% = Total Rooms Occupied/ Total Rooms Available
  
  • RevPAR (Revenue Per Available Room) = Total Revenue / Total Rooms Available to Sell
  
  • Realization = DURN/DBRN

## Preview 📊
### Booking Analysis

  ![Library_project](https://github.com/BijoyBytes/Power-Bi-Hospitality-Analysis/blob/main/Booking%20Analysis.png)

### Revenue Analysis

 ![Library_project](https://github.com/BijoyBytes/Power-Bi-Hospitality-Analysis/blob/main/Revenue%20Analysis.png)



## Recommendations
  

1. **📈 Boost Occupancy Rate**
   - **Current:** 57.8%
   - **Target:** 70%+
   - **Actions:**
     - Promote weekday stay packages and special offers.
     - Focus marketing on high-performing platforms:
       - *Tripster* – 70.1% realization
       - *Direct Online* – 69.9% realization

2. **❌ Reduce Cancellation Rate**
   - **Current:** 24.8%
   - **Target:** <15%
   - **Actions:**
     - Introduce non-refundable booking options.
     - Encourage rebooking instead of cancellations.
     - Prioritize channels with low cancellation rates:
       - *Tripster* – 21.5% cancellations

3. **🌟 Improve Guest Ratings**
   - **Current Average Rating:** 3.62
   - **Target:** 4.0+
   - **Actions:**
     - Improve service quality in low-rated cities:
       - *Mumbai* – 2.3
       - *Delhi* – 2.5
     - Solicit and act on guest feedback proactively.

4. **🛒 Optimize Booking Channels**
   - **Objective:** Increase Direct Online bookings to reduce commission costs.
   - **Current:** 5 bookings
   - **Target:** 15+ bookings
   - **Actions:**
     - Promote Direct Online channels via loyalty programs and exclusive discounts.
     - Reduce dependency on *MakeMyTrip* (currently 41 bookings).

5. **💰 Drive Revenue Growth**
   - **Current ADR:** ₹12.7K
   - **Current RevPAR:** ₹7,337
   - **Target RevPAR:** ₹8,000+
   - **Actions:**
     - Focus on high-revenue cities:
       - *Mumbai* – ₹661M revenue
       - *Hyderabad* – ₹321M revenue
       - *Delhi* – ₹291M revenue
     - Implement targeted upselling and cross-selling strategies.
