# Olympic-History-Performance-Analysis

📊 A Power BI Dashboard analyzing 120 years of the Olympic Games (1896–2016)
## 📌 Introduction
In the evolving landscape of sports analytics, historical data plays a crucial role in understanding the progression of human performance. This project bridges the gap between raw archival records and actionable insights by analyzing over 120 years of Olympic history.

Using Microsoft Power BI, this interactive dashboard visualizes participation trends, athlete demographics, and national dominance, transforming over 270,000 rows of data into a dynamic narrative of the Olympic Games.

📸 Dashboard Snapshot
(Place a screenshot of your dashboard here)

## 🎯 Project Objectives
The analysis was driven by specific objectives aimed at uncovering patterns in athletic history:

Long-Term Trends: Analyze the exponential growth of the Games and the evolution of gender ratios over time.

National Dominance: Identify top-performing nations based on medal tallies and "quality of wins" (Gold vs. Silver vs. Bronze).

Physical Analysis: Correlate athlete biometrics (Height & Weight) with success in specific sports.

Demographics: Determine the peak performance age for athletes across different disciplines.

Seasonal Evolution: Track the expansion of sports in both Summer and Winter Games.

## ⚙️ Tech Stack
Microsoft Power BI Desktop: Data ingestion, modeling, and visualization.

Power Query: ETL (Extract, Transform, Load) processes for data cleaning.

DAX (Data Analysis Expressions): Custom measures for medal counts and participation ratios.

Excel/CSV: Raw data source format.

## 📂 Dataset
The dataset was obtained from Kaggle (originally scraped from Sports-Reference.com).

Source: 120 Years of Olympic History: Athletes and Results

Coverage: 1896 – 2016

Key Columns: ID, Name, Sex, Age, Height, Weight, Team, NOC, Games, Year, Season, City, Sport, Event, Medal.

## 🧹 Data Preprocessing (ETL)
Before visualization, the raw data underwent significant cleaning in Power Query Editor:

Data Typing: Converted Age, Height, and Weight from text to numeric types, handling "NA" values.

Null Handling: Processed Medal columns to distinguish between non-medalists (NA) and medal winners.

Data Modeling: Established relationships between the main Athlete Events table and the NOC Regions dictionary to map country codes to full names.

Calculated Measures (DAX):

Total Medals = COUNTROWS(FILTER('Olympics', 'Olympics'[Medal] <> BLANK()))

Total Athletes = DISTINCTCOUNT('Olympics'[ID])

## 🔍 Key Insights & Visuals
1. Participation & Gender Trends (Stacked Area Chart)
Observation: The games have seen massive exponential growth. Female participation was nearly non-existent in the early 1900s but has narrowed the gap significantly in the 21st century.

2. Country Performance (Bar Chart)
Observation: Historically, the USA and Soviet Union have dominated the podium. The visual highlights the disparity in medal counts between developed nations with strong sports infrastructure and developing nations.

3. "Form Follows Function" (Scatter Chart)
Observation: Plotting Height vs. Weight reveals distinct clusters. Gymnasts occupy the low-height/low-weight quadrant, while Basketball players and Throwers occupy the high-height/high-weight extremes, validating biomechanical advantages.

4. Age Demographics (Column Chart)
Observation: Athlete age follows a standard bell curve, peaking in the early-to-mid 20s, indicating the prime physical window for most Olympic disciplines.

## 🚀 Future Scope
Real-Time Data: Integrate Python scripts to fetch live medal counts during future games.

Predictive Analytics: Use Machine Learning to forecast future medal tallies based on historical GDP and population data.

Granular Analysis: Incorporate event-specific data (race times, jump distances) to track the evolution of human speed and strength.

## 🤝 Credits & References
Dataset: Kaggle - 120 Years of Olympic History

Course: INT374 Data Visualization and Analytics, Lovely Professional University.

Tools: Microsoft Power BI.

## 👤 Author
Ansh Kumar Sonker

LinkedIn: https://www.linkedin.com/posts/anshsonker89_powerbi-dataanalytics-datavisualization-activity-7406261278379368448-NhSQ?utm_source=social_share_send&utm_medium=android_app&rcm=ACoAAGGNCq4BA5ToI7tpqd7A77GPCsup8RQtPRE&utm_campaign=copy_link

<img width="1788" height="811" alt="Screenshot 2025-12-15 224518" src="https://github.com/user-attachments/assets/24951280-2edd-4e35-94ee-950edd182b09" />


