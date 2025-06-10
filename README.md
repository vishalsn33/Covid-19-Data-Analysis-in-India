# Covid-19-Data-Analysis-in-India

This project is a Power BI data visualization dashboard focused on analyzing COVID-19 data for New Delhi, India. The goal is to track, visualize, and understand the impact of the pandemic using interactive charts, maps, KPIs, and gauges. The dataset includes confirmed cases, recoveries, deaths, and dates for insightful time-based analysis.

**📁 Dataset Description
Location: (India)**

Columns:

Date – Reporting date

State – Always "Delhi"

City – Always "New Delhi"

**Confirmed – Confirmed COVID-19 cases

Recovered – Recovered COVID-19 cases

Deaths – COVID-19 death count**

**⚙️ Tools & Technologies Used
Power BI Desktop – For building the dashboard**

Power Query Editor – For data cleaning and transformation

DAX (Data Analysis Expressions) – For creating custom measures

Data Modeling – Date hierarchy, measures, and filters

**📊 Power BI Visuals Used and Their Purposes
Visual Used	Purpose**
✅ KPI Card	Show main metrics like Total Confirmed, Total Deaths, Total Recovered, Active Cases
📈 Line Chart	Visualize daily or monthly trends of Confirmed, Recovered, and Death cases over time
📊 Bar Chart	Compare case types (Confirmed, Recovered, Deaths) on different dates or months
🥧 Pie Chart	Show percentage distribution of Confirmed, Recovered, and Deaths cases
🗺️ Map	Highlight New Delhi (or other cities if available) with bubble size based on total cases
🎯 Gauge Chart	Show metrics like Recovery Rate or Death Rate visually using threshold indicators
🎛️ Slicer	Allow users to filter data by Date, Month, or Year to perform dynamic filtering

**🧮 Key Measures (DAX)**
DAX
Copy
Edit
Total Confirmed = SUM('CovidData'[Confirmed])
Total Recovered = SUM('CovidData'[Recovered])
Total Deaths = SUM('CovidData'[Deaths])
Active Cases = [Total Confirmed] - [Total Recovered] - [Total Deaths]
Recovery Rate = DIVIDE([Total Recovered], [Total Confirmed], 0)
Death Rate = DIVIDE([Total Deaths], [Total Confirmed], 0)
These measures are used in KPI cards, gauge charts, and calculated insights for comparative visuals.

**💡 Dashboard Insights
📈 Trend Analysis:** Line charts showed peaks of confirmed and death cases in specific months.

**🧮 KPI Cards:** Clearly display cumulative totals and active cases in real time.

**🥧 Pie Chart:** Provided intuitive understanding of how many people recovered vs died.

**🗺️ Map View:** Even for one city (New Delhi), maps visually highlight the case density.

**🎯 Gauge Chart:** Makes it easy to monitor whether the death rate or recovery rate is in a safe range.

**🎛️ Slicers:** Allow users to filter by year or month for focused analysis.

**📅 How It Works**
Load the .pbix file in Power BI Desktop.

Click on each visual to interact with slicers and filters.

Use the Slicer to filter visuals by Date, Month, or Year.

Hover over tooltips in charts for detailed information on exact values.

Check the KPI cards for real-time totals and comparisons.

Gauge charts show recovery or mortality rate in a percentage scale.


**Dashboard-preview:  **  : https://github.com/vishalsn33/Covid-19-Data-Analysis-in-India/blob/main/Covid-19%20Data%20Analysis%20in%20India.png
🙌 Acknowledgements
Data collected for educational use

Built using Microsoft Power BI

Inspired by real-time COVID-19 dashboards used by governments and NGOs
