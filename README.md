foldername/placeholder.txt
cyclistic-q1-analysis/
├─ README.md
├─ report/
│  └─ Cyclistic_Q1_Report[full pdf report of cyclistic project.pdf](https://github.com/user-attachments/files/21808563/full.pdf.report.of.cyclistic.project.pdf)
.pdf
├─ data/
│  ├─ cleaned/
│  │  ├─ rides_by_weekday,member_casual,day_of_week,ride_length
1,casual,Sunday,5061.304364
2,member,Sunday,972.9383358
3,casual,Monday,4752.050438
4,member,Monday,822.3112017
5,casual,Tuesday,4561.803857
6,member,Tuesday,769.4416288
7,casual,Wednesday,4480.372432
8,member,Wednesday,711.9837903
9,casual,Thursday,8451.666853
10,member,Thursday,707.2092743
11,casual,Friday,6090.737302
12,member,Friday,796.7337889
13,casual,Saturday,4950.770801
14,member,Saturday,974.0729638
[avg_ride_length.csv](https://github.com/user-attachments/files/21797050/avg_ride_length.csv)
.csv
│  │  ├─ rides_,year,month_num,month,member_casual,total_rides,avg_duration
1,2019,1,January,casual,4602,2839.483485
2,2019,1,January,member,98670,939.0025844
3,2019,2,February,casual,2638,8736.29113
4,2019,2,February,member,93548,804.2173323
5,2019,3,March,casual,15923,3138.354079
6,2019,3,March,member,149688,782.4209422
7,2020,1,January,casual,7785,9698.969171
8,2020,1,January,member,136099,668.9422553
9,2020,2,February,casual,12314,7997.164609
10,2020,2,February,member,126714,768.3971621
11,2020,3,March,casual,24615,4250.223035
12,2020,3,March,member,115593,860.0643551
[rides_by_month_v2.csv](https://github.com/user-attachments/files/21797044/rides_by_month_v2.csv)
by_month.csv
│  │  └─ rides_by_season.c,season,member_casual,avg_duration
1,Spring,casual,63.55816436
2,Spring,member,13.60421873
3,Winter,casual,128.0814947
4,Winter,member,13.05014962
[rides_by_season.csv](https://github.com/user-attachments/files/21797051/rides_by_season.csv)
sv
│  └─ raw/           
│     └─ [cyclistic 2020 data.zip](https://github.com/user-attachments/files/21797073/cyclistic.2020.data.zip)
Raw_Dat[cyclistic 2019 data.zip](https://github.com/user-attachments/files/21797072/cyclistic.2019.data.zip)
a.zip
├─ scripts/
│  └─ cyclistic_cleaning_a[Cyclistic analysis with R.pdf](https://github.com/user-attachments/files/21797034/Cyclistic.analysis.with.R.pdf)
nalysis.R
├─ images/
│  ├─ dashboard_screenshot.png
│  ├─ weekda<img width="799" height="635" alt="Weekday_Analysis" src="https://github.com/user-attachments/assets/107fa81a-0599-4b77-b831-ec3326dcd950" />
y_chart.png
│  ├─ monthly<img width="1393" height="635" alt="Monthly Analysis" src="https://github.com/user-attachments/assets/21282b66-4ebf-4ef5-a613-87f6819d273b" />
_trend.png
│  └─ seasona<img width="413" height="635" alt="Seasonal Analysis" src="https://github.com/user-attachments/assets/15cf437e-fbe8-46b9-8cfb-2e08ab61e41f" />
l_chart.png
└─ tableau/
   └─ Cyclistic_Q1_Dashboard.twbx   (or link in README if on Tableau Public)
[Uploading Cyclistic Project.twb…]()

# 🚲 Cyclistic Bike-Share Analysis (Google Data Analytics Capstone)

This project is my **Google Data Analytics Capstone Case Study**, where I analyzed Cyclistic bike-share data to identify differences between **casual riders** and **annual members**, and recommend strategies to increase memberships.

---

## 📊 Project Overview
- **Business Task:** Identify how annual members and casual riders use Cyclistic bikes differently and recommend strategies to convert casuals into members.  
- **Data Source:** Public Cyclistic trip data (Q1 for 2019 & 2020).  
- **Tools Used:** R (tidyverse, lubridate), Tableau Public, Excel.  
- **Outputs:** Cleaned datasets, R scripts, Tableau dashboards, written report.

---

## 🔑 Key Findings
1. **Weekday Patterns:**  
   - Casual riders’ **average trip duration peaks on Thursday**.  
   - Members remain relatively steady across weekdays.  

2. **Monthly Patterns:**  
   - **2019:** upward trend toward March.  
   - **2020:**  
     - **Casual average duration peaks in March**.  
     - **Member average duration is lowest in March**.  

3. **Seasonal Patterns:**  
   - **Winter shows higher overall activity** than spring (in Q1).  
   - Casual riders consistently take longer rides than members.

---

## 💡 Recommendations
- **Midweek Campaigns:** “Try-a-Membership Thursday” to target casual riders when their trip duration spikes.  
- **Seasonal Targeting:** Push **late-winter/early-spring offers**, especially March when casual rides peak.  
- **Commute Value Messaging:** Highlight reliability and cost savings to members whose ride durations shorten.  
- **Winter Readiness:** Ensure bike availability and safety communications to support strong winter activity.  

---

## Files
- **Report:** `report/Cyclistic_Q1_Report.pdf`
- **Scripts:** `scripts/cyclistic_cleaning_analysis.R`
- **Data (cleaned):** `data/cleaned/*.csv`
- **Dashboard:** `tableau/Cyclistic_Q1_Dashboard.twbx` (or Tableau Public link)

## How to Reproduce
1. Open R script in `scripts/` and run to regenerate cleaned CSVs.
2. Load CSVs into Tableau; recreate visuals per README notes.
3. Or open the packaged workbook (`.twbx`) directly.

## Notes / Limitations
- Dataset covers **Q1 only** for both years.
- **Hour-of-day analysis intentionally omitted**.
