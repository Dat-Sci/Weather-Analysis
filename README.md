<<<<<<< HEAD
# Weather Trends: Comparing Daily Max & Min Temperatures (2005–2014 vs 2015)
=======
Weather Trends: Comparing Daily Max & Min Temperatures (2005-2014 vs 2015)
A time series analysis of temperature variations in Ann Arbor Michigan.
 * Maximum and minimum daily temperatures against months for each day in the year between the years 2005 and 2014, with the exceeding values of the year 2015 for the area Ann Arbor Michigan.
>>>>>>> 6bc08e3db4022d430fa97b86d11c46a67b220eda

This project analyzes **daily maximum and minimum temperature trends** in **Ann Arbor, Michigan**, comparing the decade **2005–2014** against the year **2015**.  
The goal is to identify whether temperature extremes have shifted significantly, offering insights into local climate variations over time.

<<<<<<< HEAD
---
=======
**overview**  
The focus is on understanding whether temperature extremes changed significantly and what this might indicate about local climate variation.
>>>>>>> 6bc08e3db4022d430fa97b86d11c46a67b220eda

## 📊 Overview

<<<<<<< HEAD
The analysis focuses on daily temperature patterns across multiple local weather stations in Ann Arbor.  
By grouping and visualizing temperature data over months for each day of the year, the project aims to reveal long-term patterns and highlight potential shifts in extremes.
=======
**Data Set**  
Source: https://www.ncei.noaa.gov/products/land-based-station/global-historical-climatology-network-daily
The dataset consists of the variables above for multiple stations identified in that geographical area.
Features and cleaning are described in the file in a coherent way.
>>>>>>> 6bc08e3db4022d430fa97b86d11c46a67b220eda

The dataset was chosen to explore how **temperature behavior evolved over a decade**, particularly to observe whether **the year 2015** exhibited unusual deviations compared to the preceding ten years.

<<<<<<< HEAD
---

## 🧾 Dataset
=======
**insight**  
Expectations were set to about a few points in summer for higher temperatures, and vice versa for winter periods. However, the results were surprising as "highs and lows" were more than expected and were happening all thoughout the year. For example, black points in the autumn period, and untill late winter, not many "low" points were discovered but rather "high" points with greater ratio than the low points. As an individual who is not experienced in earth's atmospheric sciences I could not find a link to real-life implications like global warming, as this visual is not enough data to conclude anything related to that. However, conclusion can be drawn as there are unexpected change in weather in terms of temperature rises and falls.

**Visual efficiency**  
* As the visual has a considerably higher ink-data ration, it uses a banalaced amount of embelishments while still focusing on functionality as the shaded area and labels makes it easier to understand and study.
>>>>>>> 6bc08e3db4022d430fa97b86d11c46a67b220eda

- **Source:** [NOAA Global Historical Climatology Network – Daily (GHCN-D)](https://www.ncei.noaa.gov/products/land-based-station/global-historical-climatology-network-daily)  
- **Location:** Ann Arbor, Michigan  
- **Period Covered:** 2005–2014 (historical baseline) and 2015 (comparison year)  
- **Variables Used:** Daily Maximum Temperature, Daily Minimum Temperature  

The dataset contains multiple weather station records from the region. Data cleaning and preprocessing steps are documented in the notebook to ensure consistency and reliability across sources.

---

## ⚙️ Data Preparation & Processing

- Loaded and merged multiple station data for Ann Arbor  
- Filtered to include only relevant variables (TMAX, TMIN)  
- Grouped data by **day of the year** to produce average daily temperature patterns  
- Created a separate subset for **2015** to compare with the baseline decade  
- Prepared the data for time-based visualization using `pandas`

---

## 📈 Visualization & Design

The project’s main visualization presents:

- **Shaded regions** representing the range between daily max and min temperatures (2005–2014)  
- **Overlaid points** showing **2015’s daily extremes** that exceeded historical bounds  
- **Month-wise x-axis** for better temporal readability  

This approach maintains a **high data-to-ink ratio**, minimizing chart clutter while emphasizing functional readability.  
Non-essential visual elements (“chart junk”) were avoided, resulting in a clean and efficient chart that communicates the temperature variations effectively.

---

## 🔍 Insights

Initial expectations were for slight temperature increases during summer and decreases in winter.  
However, the results revealed **unexpectedly frequent high-temperature anomalies** throughout the year — not just during summer months.  
For example:
- Several high outliers appeared during **autumn and late winter**, while fewer low outliers were observed.  
- These results suggest **increased irregularity** in temperature patterns.

While this visualization alone cannot confirm broader phenomena such as global warming, it does indicate **unusual and frequent deviations** in local weather patterns during 2015.

---

## 🧩 Tools & Libraries

- **Python**
- **pandas**
- **matplotlib.pyplot**