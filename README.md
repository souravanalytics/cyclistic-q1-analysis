foldername/placeholder.txt
cyclistic-q1-analysis/
├─ README.md
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

# Cyclistic Bike-Share Q1 Analysis – Driving Membership Growth

**Author:** Sourav Chakraborty  
**Tools:** R (tidyverse, ggplot2), Tableau Public, Excel

## Overview
This Google Data Analytics case study analyzes **Cyclistic** bike-share trips for **Q1 (Jan–Mar) across two years** to understand differences between **members** and **casual riders** and recommend strategies to increase memberships.

**Dashboard:** [View on Tableau Public](https://public.tableau.com/views/CyclisticProject_17550651032680/CyclisticBike-ShareMembervsCasualRiderTrends?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  

## Data
- Source: Cyclistic public trip data (Q1 for two consecutive years).
- Volume: ~1M rows (post-cleaning subset used for visuals).
- Cleaned datasets (CSV):  
  - `data/cleaned/rides_by_weekday.csv`  
  - `data/cleaned/rides_by_month.csv`  
  - `data/cleaned/rides_by_season.csv`  

## Method
1. **Prepare (R):** remove nulls/dupes, fix datetimes, create `ride_length`, `day_of_week`, `month`, `month_num`, `year`, `season`.
2. **Aggregate (R):** three tidy tables for Tableau (weekday, monthly, seasonal).
3. **Visualize (Tableau):** separate worksheets → one dashboard.

## Key Findings (Q1 only)
- **Ride Duration:** Casual rides are longer on average than member rides.
- **Weekday vs Weekend:** Members are steady on weekdays; casual riders peak on weekends.
- **Seasonality:** March uptick for both segments; spring boosts casual activity.

## Recommendations
- **Weekend promotions** for casual riders.
- **Spring campaigns** to convert casuals before summer.
- **Trial memberships** to reduce friction.

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

## License
MIT License. See `LICENSE`.
