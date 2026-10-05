# LOGISTICS OPERATIONS ANALYTICS

#  Executive Summary

This project delivers an end-to-end analysis of logistics operations, connecting **service reliability, route performance, driver efficiency, fleet utilisation, and operating costs** to provide a unified view of operational and financial performance.

The analysis reveals a business generating **$262.53M in revenue across more than 85,000 loads**, but facing significant operational inefficiencies. Only **44.61% of deliveries were completed on time**, with late deliveries averaging approximately **180 minutes behind schedule**. Detention was also widespread at **88.65%**, highlighting persistent service and facility-level challenges across the network.

From an operational perspective, driver idle time averaged approximately **28%**, while maintenance costs and downtime were concentrated among specific fleet assets. Financially, **fuel emerged as the dominant identified operating cost at $95.59M**, significantly outweighing maintenance expenditure and making fuel efficiency a major opportunity for cost optimisation.

The analysis ultimately highlights a central business opportunity: **improving profitability does not depend solely on increasing shipment volume or revenue, but on operating the existing network more efficiently.** Reducing fuel exposure, improving delivery reliability, addressing detention, and targeting high-cost fleet assets provide clear opportunities to strengthen both operational performance and financial outcomes.

# Business Objective

The objective of this project is to evaluate the **operational efficiency, service reliability, and financial performance** of the logistics network to identify the factors associated with delivery delays, operating costs, and asset underperformance.

The analysis focuses on connecting performance across **drivers, routes, fleet assets, customers, facilities, fuel consumption, maintenance, and safety** to provide management with a comprehensive view of the logistics operation.

The key objectives are to:

- Assess overall **revenue, shipment volume, and service performance**.
- Identify **routes and facilities** associated with poor delivery performance and high detention.
- Evaluate **driver performance and fuel efficiency** using metrics such as MPG, idle time, on-time delivery, and safety incidents.
- Assess **fleet utilisation and asset performance**, including maintenance costs and downtime.
- Analyse **fuel, maintenance, and safety-related costs** and their impact on financial performance.
- Evaluate **customer revenue and service levels** to identify commercially important areas exposed to poor delivery reliability.
- Identify **seasonal and monthly performance patterns** across revenue, load volume, service reliability, and operating contribution.
- Translate operational findings into **actionable recommendations** that can improve efficiency, service delivery, and financial performance.

# Data Architecture & Tools

## Data Source:

The dataset used for this analysis is available here:  
[Logistics Operations Dataset](https://drive.google.com/drive/folders/1Uk7U-DvssMWGyBxSaXHo-TqzanptUJZf?us)

The dataset consists of **14 interconnected tables** covering key areas of logistics operations, including **loads, trips, customers, routes, drivers, trucks, trailers, facilities, delivery events, fuel purchases, maintenance records, safety incidents, driver performance, and truck utilisation**.

These datasets were integrated to analyse **service reliability, route performance, driver efficiency, fleet utilisation, fuel consumption, maintenance activity, safety performance, customer service levels, and operating costs** across the logistics network.

---

## Tools and Technologies Used:

- **Microsoft Excel** → Initial data exploration, validation, and understanding of the source datasets
- **Power BI** → Primary tool for data analysis, data modelling, interactive dashboard development, and executive reporting
- **Power Query** → Data cleaning, transformation, data type validation, and preparation of the 14 datasets for analysis
- **DAX (Data Analysis Expressions)** → Creation of calculated columns and measures for KPIs such as **On-Time Delivery Rate, Revenue per Mile, Average MPG, Idle Time %, Detention Rate, Maintenance Cost per Mile, Incident Rate, and Operating Contribution**
- **Data Modeling** → Development of a **fact constellation model**, connecting operational fact tables with shared dimensions such as Customers, Routes, Drivers, Trucks, Facilities, and Date
- **Date Table** → Created to support consistent time-based analysis and identify monthly and seasonal performance patterns
- **PowerPoint** → Dashboard wireframing, layout planning, and visual storytelling before development in Power BI
- **GitHub** → Project documentation, portfolio presentation, and presentation of the final analytical solution

# Executive Dashboards & Analysis

The Power BI solution is structured across **four interconnected analytical dashboards**, each designed to answer a specific business question. Together, the dashboards move from identifying overall performance issues to understanding **where they occur, what operational factors are associated with them, and their financial impact**.

---

## 1. Executive Overview

**Business Question:**  
> *How is the logistics business performing overall, and are customers receiving reliable service?*

The Executive Overview provides a high-level view of the network's **commercial performance, shipment activity, service reliability, and financial efficiency**.

### Key Findings:

- The logistics network generated **$262.53M in total revenue** across approximately **85K loads**.
- Revenue remained relatively stable across the reporting period, indicating consistent commercial activity.
- Despite strong revenue generation, only **44.61% of deliveries were completed on time**, meaning approximately **55% of deliveries were late**.
- Late deliveries averaged approximately **180 minutes behind schedule**, showing that delays were substantial rather than marginal.
- The business generated approximately **$2.15 in revenue per mile**.
- Operating Contribution Margin stood at approximately **61.40%**, based on the operating costs identifiable within the dataset.
- Monthly load volumes remained relatively stable while on-time performance continued around the mid-40% range, indicating that service reliability remained a persistent issue.

**Key Insight:**  
> Strong revenue and shipment activity are being achieved alongside consistently weak delivery reliability, creating a need to investigate where service underperformance is concentrated.

![Executive Overview Dashboard](https://github.com/Akinlade-Opeyemi-Mary/Logistics-Operations-Analytics/blob/d6cd00745eeeab6c0b690855e5da5afa656749f9/EXCEUTIVE%20OVERVIEW%20DASHBORD.png?raw=true)
---

## 2. Service & Route Performance

**Business Question:**  
> *Where is service underperformance concentrated, and what operational factors are associated with it?*

This dashboard investigates delivery performance across **routes, facilities, and customers**, connecting service reliability with detention and route-level operating efficiency.

### Key Findings:

- Approximately **47K deliveries were late**, with an overall on-time delivery rate of only **44.61%**.
- Late deliveries averaged approximately **180 minutes behind schedule**.
- Route-level analysis shows consistently weak on-time performance across several lanes, with relatively limited variation between the poorest-performing routes.
- Detention was widespread, with an overall **88.65% detention rate**.
- Total detention hours were particularly concentrated at facilities including the **Nashville Distribution Center, Atlanta Warehouse, and Detroit Hub**.
- Customer-level analysis shows that commercially important customers are also exposed to weak service reliability.
- Route-level fuel cost analysis identifies specific lanes with comparatively high fuel cost per mile, highlighting areas where service and operating efficiency can be reviewed together.

**Key Insight:**  
> Service underperformance is not isolated to a single route or customer. Delivery delays and detention occur across the network, while specific routes and facilities provide clear areas for targeted operational intervention.

---

## 3. Driver & Fleet Performance

**Business Question:**  
> *How efficiently are drivers and fleet assets being utilised, and where are performance issues concentrated?*

The Driver & Fleet dashboard evaluates **driver efficiency, fuel performance, safety, maintenance expenditure, and fleet downtime** to identify areas of operational underperformance.

### Key Findings:

- Drivers achieved an average fuel efficiency of approximately **6.45 MPG**.
- Approximately **28% of total trip duration was recorded as idle time**, indicating an opportunity to improve driver and fuel efficiency.
- Driver-level analysis identifies individuals with comparatively high idle-time percentages.
- Performance analysis by driver experience compares **MPG, idle time, on-time delivery, trip productivity, and safety performance**, highlighting differences across experience groups.
- Maintenance expenditure is concentrated among specific trucks, with the highest-cost assets generating approximately **$72K–$90K in maintenance costs**.
- Fleet downtime is similarly concentrated, with the most affected trucks recording approximately **940–1,133 hours of downtime**.
- Safety incidents are concentrated among particular drivers, allowing safety intervention to be targeted rather than applied uniformly across the workforce.
- The analysis also identified **1,672 unmatched truck trips**, highlighting an additional area for operational and data-quality review.

**Key Insight:**  
> Driver and fleet performance is not uniform. Specific drivers and assets account for disproportionate levels of idle time, maintenance expenditure, downtime, and safety exposure, creating opportunities for targeted performance management.

---

## 4. Financial Impact

**Business Question:**  
> *What is driving operating costs, and where are the greatest opportunities to protect financial performance?*

The Financial Impact dashboard connects the operational findings to their financial consequences, providing management with a clearer view of **revenue, operating contribution, and major cost drivers**.

### Key Findings:

- The logistics network generated **$262.53M in total revenue**.
- Approximately **$161.20M in Operating Contribution** was generated after accounting for the operating costs included in the contribution calculation.
- Operating Contribution Margin stood at approximately **61.40%**.
- Fuel expenditure reached approximately **$95.59M**, making fuel the dominant identified operating cost.
- Maintenance expenditure totalled approximately **$5.73M**.
- Fuel represented approximately **90% of the fuel, maintenance, and safety-related costs analysed**, making fuel efficiency the largest identifiable cost optimisation opportunity.
- Operating contribution remained relatively stable across the reporting period, reinforcing the importance of protecting existing financial performance through greater operational efficiency.

> **Note:** Operating Contribution should not be interpreted as accounting net profit, as the dataset does not contain all business expenses such as wages, insurance, depreciation, tolls, and administrative costs.

**Key Insight:**  
> Financial performance is most exposed to fuel expenditure and wider operational inefficiencies. Improving route efficiency, reducing excessive idle time, addressing detention, and targeting high-cost fleet assets provide the clearest opportunities to strengthen operating contribution.
