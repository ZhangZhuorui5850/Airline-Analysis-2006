# Airline-Analysis-2006
This project analyzes U.S. domestic flight performance in **2006** using the Airline On-Time Performance dataset. It focuses on uncovering **patterns of delays and cancellations** using Hive SQL and Python-based visualization.

The analysis is structured into four major sections.

---

## 📁 Project Structure

| Notebook | Description |
|----------|-------------|
| `Q1_DelayPatterns.ipynb` | Analysis of departure delays by **time of day**, **day of week**, and **month** |
| `Q2_DelayFactors.ipynb`  | Investigation of the top 5 causes of delays (Carrier, Weather, NAS, Security, Late Aircraft) |
| `Q3_CancellationAnalysis.ipynb` | Breakdown of cancellations by **reason**, **airline**, **airport**, **month**, and **time of day**, with map visualization |
| `Q4_ProblematicRoutes.ipynb` | Identification of **problematic routes**, **flight numbers**, and **carriers**, plus extended analysis of delay patterns by time and airport |

Each notebook contains:
- Hive SQL queries using Impala
- Pandas + Seaborn/Matplotlib visualizations
- Markdown commentary and insights

---

## 📦 Dataset

The full dataset (~600MB) is not included due to GitHub file size limitations.

You can download the 2006 flight data from Kaggle:  
🔗 https://tinyurl.com/u8rzvdsx

Please refer to the instructions in [`data/README.md`](./data/README.md) for how to load it into Hive.

---
## 📘 Full Analysis Summary
 [Go to Full Analysis Summary](docs/Analysis_Summary.md)


