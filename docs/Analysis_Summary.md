# 📊 2006 U.S. Flight Delay and Cancellation Analysis Summary

This project uses Hive SQL and Python visualizations to analyze the delay and cancellation patterns of domestic flights in the United States in 2006, focusing on temporal patterns, delay causes, cancellation reasons, and high-risk routes and carriers.

---

## 🟢 Q1: Temporal Distribution of Flight Delays

**Objective:** Analyze the average departure delay at different times of day, days of the week, and months to identify high-risk time periods.

### Key Findings:

- **Time of Day:**
  - Early morning flights (6–9 AM) experience the least delay;
  - Delays increase in the afternoon and evening, averaging over 20 minutes from 15:00 to 23:00.
  
  ![](../figures/Average%20Departure%20Delay%20by%20Time%20of%20Day.png)  
  *Figure 1: Average departure delay by time of day*

- **Day of Week:**
  - Tuesday and Wednesday flights are most punctual;
  - Friday and Sunday delays are severe due to business and weekend travel.

  ![](../figures/Average%20Departure%20Delay%20by%20Day%20of%20Week.png)  
  *Figure 2: Average departure delay by day of week*

- **Month:**
  - July and December are peak months for delays (holidays + weather);
  - February delays are also significant due to winter storms.

  ![](../figures/Average%20Departure%20Delay%20by%20Month.png)  
  *Figure 3: Monthly average departure delay*

---

## 🟠 Q2: Comparison of Five Delay Types

**Objective:** Compare the frequency, total delay time, and average delay time for five delay causes: Carrier, Weather, NAS, Security, and Late Aircraft.

### Key Findings:

- **Most total delay time:**
  - Late Aircraft delay far exceeds other categories.

  ![](../figures/Total%20Delay%20Time%20by%20Cause%20(in%20Minutes).png)  
  *Figure 4: Total delay time by cause*

- **Highest average delay:**
  - Security delays are rare but average over 60 minutes;
  - Weather delays are highly variable.

  ![](../figures/Average%20Delay%20Time%20per%20Event%20by.png)  
  *Figure 5: Average delay time by cause*

- **Monthly trend:**
  - Multiple delay types spike in July and December.

  ![](../figures/Frequency%20of%20Delay%20Events%20by%20Cause.png)  
  *Figure 6: Monthly distribution of delay events by cause*

---

## 🔵 Q3: Flight Cancellations – Reasons and Patterns

**Objective:** Analyze key cancellation causes, temporal trends, airline differences, and spatial distribution across airports.

### Key Findings:

- **Main cancellation causes:**
  - Weather is the most common, followed by Carrier and NAS.

  ![](../figures/Flight%20Cancellations%20by%20Reason.png)  
  *Figure 7: Distribution of cancellation reasons*

- **Monthly trend:**
  - February (snowstorms) and June (thunderstorms) show cancellation peaks.

  ![](../figures/Flight%20Cancellation%20Rate%20by%20Month.png)  
  *Figure 8: Monthly cancellation trend*

- **High-risk airports:**
  - ORD (Chicago) and ATL (Atlanta) have high cancellation rates;
  - Map shows Northeast and Midwest as cancellation hotspots.

  ![](../figures/Top%2030%20Airports%20by%20Cancellation%20Rate.png)  
  *Figure 9: Cancellation rate by airport*

- **Time of day:**
  - Evening and night flights are more likely to be canceled, likely due to operational backlogs.

  ![](../figures/Flight%20Cancellation%20Rate%20by%20Time%20of%20Day.png)  
  *Figure 10: Cancellation rate by time of day*

---

## 🟣 Q4: High-Delay Routes, Flight Numbers, and Airlines

### Q4.1: Routes with Highest Cancellation Rates

- Many routes ending in ORD top the cancellation list.

  ![](../figures/Top%2015%20Routes%20by%20Flight%20cancellation%20Rate.png)  
  *Figure 11: Top 15 routes by cancellation rate*

### Q4.2: Routes with Longest Average Delays

- Routes such as ORD → CAE exceed 34 minutes in average departure delay.

  ![](../figures/Top%2015%20Routes%20by%20Average%20Departure%20Delay.png)  
  *Figure 12: Top 15 routes by average delay*

### Q4.3: Airline Cancellation Performance

- MQ and YV have the highest cancellation rates;
- EV shows both high delay and high cancellation.

  ![](../figures/Flight%20Cancellation%20Rate%20by%20Carrier.png)  
  *Figure 13: Cancellation rate by carrier*

  ![](../figures/Average%20Departure%20Delay%20by%20UniqueCarrier.png)  
  *Figure 14: Delay by carrier*

### Q4.4: High-Delay Flight Numbers and Airport Mapping

- Flights 7465, 7458, and 7426 each average over 50 minutes in delay.

  ![](../figures/Top%2030%20Flight%20Numbers%20with%20Highest%20Avg%20Departure%20Delay.png)  
  *Figure 15: Top 30 delayed flight numbers*

#### Extension 1: Time of Departure

- Flights departing between 0–2 AM have the worst delays.

  ![](../figures/Average%20Delay%20by%20Departure%20Hour%20(Top%20Delayed%20Flight%20Numbers).png)  
  *Figure 16: Delay by hour for worst flights*

#### Extension 2: Airport Origin Distribution

- High-delay flights often depart from ORD, EWR, and MBS.

  ![](../figures/Avg%20Departure%20Delay%20by%20Origin%20(Top%20Delayed%20Flight%20Numbers).png)  
  *Figure 17: Delay by origin airport*

  ![](../figures/Airport%20Delay%20Map-Avg%20Departure%20Delay%20by%20Origin%20&%20Flight.png)  
  *Figure 18: Delay distribution map for worst flights*

---

## ✅ Conclusion and Recommendations

- **Passenger Tips:** Choose early morning flights, avoid weekends and peak holidays, and be cautious when flying from weather-sensitive hubs (e.g., Chicago, NYC).
- **Airline Strategy:** Improve buffer and rescheduling strategies to address cascading delays from Late Aircraft.
- **Future Work:** Incorporate weather and passenger volume data to enhance delay prediction accuracy.

This project demonstrates how data analytics can be used to identify risks in flight operations and optimize both airline scheduling and passenger decision-making.
