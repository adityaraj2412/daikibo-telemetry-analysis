# 📊 Daikibo Telemetry Data Analysis (Tableau Project)

## 🔹 Overview
This project analyzes telemetry data collected by **Daikibo factories** using Tableau.  
The goal was to calculate machine downtime caused by unhealthy device statuses and visualize the results.

---

## 🛠️ Tools & Skills
- Tableau (Dashboarding & Visualization)
- Data Cleaning & Transformation
- JSON Data Handling

---

## 📂 Dataset
- Source: `daikibo-telemetry-data.json` (sample telemetry data)
- Each record represents device health status in different factories.

---

## ⚙️ Methodology
1. Imported JSON data into Tableau.
2. Created a **calculated field "Unhealthy"**:
   ```tableau
   IF [status] = "unhealthy" THEN 10 ELSE 0 END
   ```
   (10 minutes downtime for each unhealthy log).
3. Built two visualizations:
   - **Down Time per Factory**
   - **Down Time per Device Type**
4. Created an interactive **Dashboard**:
   - Selecting a factory filters device-type downtime.
   - Helps identify worst-performing factory & device type.

---

## 📊 Dashboard (Screenshot)
### Factory vs Device Type
![Dashboard Screenshot](/dashboard.png)

---

## 🔍 Insights
- The **Seiko factory** recorded the highest downtime.
- Within Seiko, **LaserWeld devices** contributed most to failures.
- Actionable insight: Prioritize preventive maintenance on LaserWeld devices at Seiko.

---

## 🚀 Key Takeaways
- Learned **Tableau dashboards & filters**.
- Practiced **turning telemetry data into business insights**.
- Great example of **Data Analytics + Visualization** for manufacturing.

---

⭐ If you found this useful, connect with me on [LinkedIn](https://www.linkedin.com/in/raj24aditya) 🚀
