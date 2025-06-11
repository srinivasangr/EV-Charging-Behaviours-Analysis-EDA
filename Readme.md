🔌 EV Charging Events – Exploratory Data Analysis (EDA)
📊 Project Overview
This project presents a detailed Exploratory Data Analysis (EDA) of electric vehicle (EV) charging session data collected from 16 different charging locations. The analysis was conducted as part of a data science internship role to uncover patterns in energy consumption, charging duration, power rates, and usage behavior across different chargers and timeframes.

📁 Dataset Description
The dataset contains 277 EV charging events with the following key features:

Start Time: Timestamp when the charging session started.

Meter Start & Meter End: Energy meter readings at the start and end (in Wh).

Meter Total: Total energy transferred (in Wh).

Total Duration: Duration of the charging session (in seconds).

Charger Name: Identifier for each charging location.

🧹 Data Cleaning & Transformation
Removed entries with 0 Wh energy transfer or 0-second durations.

Converted:

Energy to kilowatt-hours (KWh)

Duration to hours

Timestamps to datetime formats

Engineered new features:

End Time, Hour of Day, Day of Week

Power Rate (KW) = Energy (KWh) / Duration (hr)

Charger_ID for sorting and visualization consistency

📈 Key Visualizations
Total Energy Consumption per Charger

Boxplots of Charging Duration and Power Rate

Hourly Charging Trends

Weekly Charging Activity

Charger-wise Charging Behavior Summary

🔍 Key Insights
Charger 4 exhibited the highest utilization.

Charger 11 may support rapid charging with power rates exceeding 100 KW.

Monday shows peak activity, suggesting weekly preparation behavior.

Anomalous durations (>25 hours) indicate potential logging issues or non-EV uses.

Most chargers support slow to medium charging aligned with typical residential behavior.

The average energy transfer per session is ~9.66 KWh.

📌 Technologies Used
Python (Pandas, Matplotlib, Seaborn)

Jupyter Notebook

PDF Report (for business presentation)

Visual analysis through bar plots, boxplots, and histograms

📂 Project Structure
bash
Copy
Edit
EDA_Charging_Events/
│
├── EDA.ipynb                    # Python notebook with step-by-step analysis
├── EDA charging events.ipynb    # Alternative version (if any updates made)
├── Srinivasan_EDA_Report.pdf    # Final report in PDF format
└── README.md                    # Project overview and documentation
🏁 Conclusion
This EDA uncovers patterns in EV charging behaviors that can aid stakeholders in:

Optimizing charger deployment and capacity

Identifying infrastructure gaps

Planning maintenance based on utilization trends

Detecting anomalies and improving data quality logging systems

