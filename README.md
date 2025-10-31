# Weather Trends: Comparing Daily Max & Min Temperatures (2005–2014 vs 2015)

This project analyzes **daily maximum and minimum temperature trends** in **Ann Arbor, Michigan**, comparing the decade **2005–2014** against the year **2015**.  
The goal is to identify whether temperature extremes have shifted significantly, offering insights into local climate variations over time.

---

## 📊 Overview

The analysis focuses on daily temperature patterns across multiple local weather stations in Ann Arbor.  
By grouping and visualizing temperature data over months for each day of the year, the project aims to reveal long-term patterns and highlight potential shifts in extremes.

The dataset was chosen to explore how **temperature behavior evolved over a decade**, particularly to observe whether **the year 2015** exhibited unusual deviations compared to the preceding ten years.

---

## 🧾 Dataset

- **Source:** [NOAA Global Historical Climatology Network – Daily (GHCN-D)](https://www.ncei.noaa.gov/products/land-based-station/global-historical-climatology-network-daily)  
- **Location:** Ann Arbor, Michigan  
- **Period Covered:** 2005–2014 (historical baseline) and 2015 (comparison year)  
- **Variables Used:** Daily Maximum Temperature, Daily Minimum Temperature  

The dataset contains multiple weather station records from the region. Data cleaning and preprocessing steps are documented in the notebook to ensure consistency and reliability across sources.

---

## ⚙️ Data Preparation & Processing

- Loaded and merged multiple station data for Ann Arbor  
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