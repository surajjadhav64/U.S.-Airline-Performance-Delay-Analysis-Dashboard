# ✈️ U.S. Airline Performance & Delay Analysis Dashboard
## 1. Project Title / Headline

**U.S. Airline Performance Dashboard: Comprehensive Flight Delay & Operational Insights**  

An interactive aviation analytics dashboard built using Power BI to analyze U.S. domestic flight data, uncovering patterns in delays, cancellations, airline   efficiency, and airport performance.

---

## 2. Short Description / Purpose  

The U.S. Airline Performance Dashboard is a data analytics project designed to explore and visualize large-scale flight data across the United States.
It helps users:
Understand flight delays and cancellations
Evaluate airline and airport performance
Analyze monthly trends and operational efficiency

This dashboard enables data-driven decision-making in aviation analytics and improves understanding of real-world transportation challenges.

---

## 3. Tech Stack 

The dashboard was built using the following tools and technologies:

Microsoft SQL Server – Used for handling large-scale data (~5.2M records), data cleaning, transformation, and integration.  
SQL (T-SQL) – Advanced querying, joins, aggregations, and KPI preparation.  
Power BI Desktop – Data visualization and dashboard development.  
Power Query – Minor transformations and data loading.  
DAX (Data Analysis Expressions) – KPI calculations (OTP rate, delays, cancellation rate).  
Data Modeling – Relationships between flights, airlines, and airports.  
Data Source Format – CSV files (flights, airlines, airports).  
Dashboard Output – .pbix file and dashboard screenshots.

---

## 4. Data Source

Source: U.S. Flight Delay & Cancellation Dataset (2015)

Dataset Includes:
Flights Data – Flight timings, delays, cancellations
Airlines Data – Airline codes and names
Airports Data – Airport details (location, city, state)
Key Columns:
Flight Date (Year, Month, Day)
Airline Code
Origin & Destination Airports
Arrival & Departure Delay
Cancellation Status & Reason
Delay Types:
Weather Delay
Airline Delay
Air System Delay
Security Delay
Late Aircraft Delay

---

## 5.Data Processing & Preparation

Due to the large dataset size (5.2+ million records), preprocessing was performed in Microsoft SQL Server to ensure efficiency and scalability.

Key Steps Performed:  
1. Data Import  
Imported CSV files into SQL Server tables:  
Flights  
Airlines  
Airports  

2. Data Cleaning  
Handled NULL values in delay columns  
Cleaned inconsistent and missing records  
Standardized column formats
 
3. Date & Time Transformation  
Converted raw time fields (HHMM format) into proper DATETIME  
Created new column:   
FLIGHT_DATE for time-based analysis

4. Data Enrichment  
Mapped cancellation codes to readable values:  
A → Airline  
B → Weather    
C → Air System  
D → Security

---

## 6. Features / Highlights

### Business Problem :  
Flight delays and cancellations:  
Impact passenger experience
Increase operational costs
Affect airline reputation

Raw data makes it difficult to answer:  
Which airlines perform best?  
What causes most delays?  
Which airports face highest delays?  
How performance changes over time?  

### Goal of the Dashboard :  
Provide a centralized analytics platform  
Compare airline performance  
Analyze delay & cancellation patterns  
Identify key operational bottlenecks  
Support data-driven decisions  

---

### Walkthrough of Key Visuals :  

#### Key KPIs (Top Section) :    
- Total Flights: 5.82M  
- OTP Rate: 82.4%  
- Avg Arrival Delay: 12.09 mins  
- Avg Departure Delay: 12.11 mins  
- Cancelled Flights: 89.88K  
- Cancellation Rate: 1.54%  
- Provides a quick snapshot of overall performance.  

---

#### Cancellation Analysis :    
- Weather is the leading cause (~49K cancellations)  
Followed by:  
- Airline issues  
- Air system delays  
- Security (minimal impact)  
- Helps identify major disruption factors  

---

#### Airline Performance :   
- OTP comparison across airlines  
- Average delay by airline  
- Helps identify:  
- Best performing airlines  
- Worst delay contributors  

---

#### Delay Distribution (Donut Chart) :   
- Breakdown of delay causes:  
- Airline delay  
- Weather delay  
- Air system delay  
- Late aircraft delay  
- Security delay  

Shows percentage contribution of each delay type

---

#### Monthly Trends :  
- OTP rate by month  
- Total flights per month  
- Helps understand:  
- Seasonal performance trends  
- Peak operational months  

---

#### Airport Performance :  
- Avg arrival delay by airport  
- OTP rate by airport  
- Identifies:
- High-delay airports
- Best-performing airports

---

#### Filters / Slicers :   
- Month  
- Airline Name  
- Airline Code  
- Origin Airport  
- Destination Airport  
Enables interactive analysis.    

---

### Business Impact & Insights :  
Key Insights  
- Weather is the biggest cause of cancellations  
- OTP rate is above 80%, indicating stable performance  
- Some airlines consistently perform better than others  
- Certain airports show higher delay patterns  
- Slight fluctuations in OTP across months  

### Strategic Insights  
- Airlines can:  
- Improve operational planning  
- Optimize aircraft scheduling  
- Airports can:  
- Reduce congestion  
- Improve infrastructure  
- Decision Support

Enables:  
- Performance benchmarking  
- Operational improvements  
- Better passenger experience  

---

## 7.Dashboard Preview
<img width="1286" height="716" alt="U S  Airline Overview" src="https://github.com/user-attachments/assets/63399990-b314-401f-9977-975ab86130c6" />

