# ✈️ Flight Operational Difficulty Analysis – Data Analytics Project

## 🏆 Project Information
- **Event:** United Airlines SkyHack 3.0  
- **Team Name:** Stat Pirates  
- **Category:** Data Analytics – Flight Delay Prediction & Insights  
- **Team Members:**  
  - Ritvik Kumar  
  - Rujhan N Sharma

## 📘 Overview
Flight delays are one of the most critical challenges in aviation, impacting passenger satisfaction, airline operations, and overall efficiency.  
This project performs an in-depth **Exploratory Data Analysis (EDA)** on flight operation data to identify **key causes of flight delays**, assess **operational efficiency**, and suggest **data-driven solutions** to minimize disruptions.
The dataset used in this project was provided by United Airlines for their Data Analytics Hackathon, called SkyHack 3.0.

---

## 🎯 Objectives
The main goals of this project are:
- To analyze the operational and service-related factors contributing to flight delays.
- To study patterns in **flight difficulty, baggage handling, special service requests, and scheduling**.
- To visualize trends in daily operations and understand correlations between different performance metrics.
- To provide actionable insights and recommendations for improving airline punctuality and efficiency.

---

## 🧩 Dataset Description
The dataset contains detailed information about flight schedules, passenger services, baggage handling, and performance indicators.

### **Key Columns**
| Category | Column Names | Description |
|-----------|---------------|-------------|
| **Flight Info** | `FLIGHT_NUMBER`, `SCHEDULED_DEPARTURE_DATE_LOCAL`, `SCHEDULED_ARRIVAL_STATION_CODE` | Identifiers and timings for each flight |
| **Performance Metrics** | `ARRIVAL_DELAY_MINUTES`, `DEPARTURE_DELAY_MINUTES`, `TURN_TIME_VIOLATION_FLAG` | Indicators of flight performance |
| **Passenger Services** | `PEOPLE_OPTED_FOR_MANUAL_WHEELCHAIR`, `PEOPLE_OPTED_FOR_ELECTRIC_WHEELCHAIR`, `PEOPLE_OPTED_FOR_UNACCOMPANIED_MINOR` | Special service requests |
| **Baggage Handling** | `TOTAL_BAGS`, `TRANSFER_BAGGAGE`, `HOT_TRANSFER_BAGGAGE` | Luggage and transfer bag statistics |
| **Operational Scores** | `FLIGHT_DIFFICULTY_SCORE`, `GROUND_TIME_SCORE`, `BAGGAGE_SCORE`, `PASSENGER_SERVICE_SCORE` | Complexity and performance ratings |
| **Passenger Demographics** | `TOTAL_PASSENGERS`, `TOTAL_BASIC_ECONOMY`, `TOTAL_STROLLER_USERS`, `TOTAL_LAP_CHILD` | Passenger segmentation |

---

## 🧠 Data Preprocessing
Before analysis, several data cleaning and transformation steps were applied:
1. **Data Normalization:** Column names converted to lowercase for consistency.  
2. **Handling Missing Values:** Missing entries in delay and service columns were filled or removed appropriately.  
3. **Data Type Conversion:** Converted date columns to datetime and numerical columns to integers/floats.  
4. **Feature Engineering:**  
   - Created new features like `Total Special Services`, `Flight Difficulty Category`, and `Route` (origin → destination).  
   - Grouped and aggregated flight-level data to daily summaries for pattern analysis.

---

## 📊 Exploratory Data Analysis (EDA)

### **1. Flight Delay Trends**
- Analyzed **daily count of delayed flights** to identify peaks and operational bottlenecks.  
- Observed highest delay count on **August 10 (382 delays)** — possible congestion or weather interference.  
- Average daily delays range between **150–380 flights**.

### **2. Last-Minute Baggage Behavior**
- **Daily average last-minute checked bags** ranged between **50–80 per day**.
- Peak observed on **August 9 (80 bags)** — correlated with highest delay count.
- Indicates a relationship between **late baggage processing and flight delays**.

### **3. Flight Difficulty Score (FDS)**
- Majority of flights had **FDS between 0.1–0.2**, representing low-complexity operations.
- Only **a few high-difficulty flights (FDS > 0.5)** were observed.
- Daily stacked bar charts revealed stable operational distribution across **Easy**, **Medium**, and **Hard** categories.

### **4. Passenger Service Usage**
- **Airport Wheelchair services** dominated (≈86% of total SSRs).  
- **Manual Wheelchairs** (7.1%) and **Unaccompanied Minors** (5.8%) had moderate usage.  
- Indicates high dependency on ground assistance and accessibility support.

### **5. Passenger Demographics**
- **Basic Economy passengers** formed the majority across all days.
- **Lap children** and **stroller users** remained consistent, reflecting steady family travel patterns.

---

## ⚙️ Correlation Analysis
- Positive correlation between **Flight Difficulty Score** and **Average Delay** — complex flights are more prone to late arrivals.
- Strong link between **Transfer Baggage Load** and **Ground Time Violation**.
- Routes with higher **Operational Complexity Scores** showed greater **delay variance**.

---

## 🧾 Key Findings
- Most delays stem from **airport congestion**, **baggage inefficiencies**, and **tight ground schedules**.  
- **Last-minute operations** (bookings, baggage) are strongly associated with departure delays.  
- **Accessibility services** add predictable but manageable boarding time extensions.  
- High FDS routes consistently show longer delays, indicating operational strain.  

---

## ✅ Recommendations

### **Operational Improvements**
- Add **buffer time** in turnaround schedules for high-complexity flights.  
- Deploy **real-time ground tracking systems** for baggage and boarding operations.  
- Use **predictive delay models** to anticipate disruptions based on weather, route, and FDS.  

### **Passenger Handling**
- Improve **special service management** via pre-scheduling and dedicated staff.  
- Streamline **boarding flow** for wheelchair and minor assistance passengers.  

### **Infrastructure Enhancements**
- Invest in **automated baggage systems** and **AI-driven logistics planning**.  
- Use **airport congestion heatmaps** to redesign time slots and reduce peak overlap.  

### **Data-Driven Planning**
- Incorporate **historical delay data** into flight scheduling algorithms.  
- Implement **Collaborative Decision-Making (A-CDM)** between airlines and ATC for better resource utilization.  

---

## 📈 Tools & Libraries Used
- **Python Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`  
- **Visualization:** Bar charts, heatmaps, pie charts, and line graphs for comparative analysis  
- **Data Handling:** GroupBy aggregations, feature engineering, and categorical binning  

---

## 💡 Conclusion
The analysis reveals that flight delays are primarily driven by **operational complexity**, **ground handling inefficiencies**, and **airport congestion**.  
By integrating **predictive analytics**, improving **baggage and passenger service management**, and adopting **data-driven scheduling**, airlines can reduce average delays by **15–25%** across key routes.

---

## 👨‍💻 Authors
**Ritvik Kumar** | *B.Tech Electrical Engineering DTU, Batch of 2026* 

📧 Email: ritvikkumar.official04@gmail.com 

🔗 [LinkedIn Profile](https://www.linkedin.com/in/ritvik-kumar-782b5324a/) 

**Rujhan N Sharma** | *B.Tech Electrical Engineering DTU, Batch of 2026* 

📧 Email: rujhansharmaa@gmail.com 

🔗 [LinkedIn Profile](https://www.linkedin.com/in/rujhan-sharma-b59628256/)

