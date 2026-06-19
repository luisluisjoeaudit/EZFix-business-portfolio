# EZFix-business-portfolio
This repository showcases "EZFix" technical branch used to automate monthly sales reporting, client issues, stocks, revenue, and the synchronization between our clients and databases. 


## Our Impact
Initially, our business relied on a n8n server to allow our clients to input their device model and hardware defects, with only a 50% success rate of transferring the data into a designated Google Calender. By using n8n's intergrated Telegram service, we were able to 
* **The Solution:** A Python pipeline that extracts, cleans, and formats data directly into an interactive Excel dashboard.
* **The Impact:** Reduced processing time by [e.g., 90%] and eliminated human data-entry errors.

Quick Navigation
* [Excel Portfolio](EXCEL-PORTFOLIO.md)
---

##  Artitechure 
* **Python:** Handles automated data extractions and calculations through primarily utilizing `pandas` .
* **Excel (`.xlsx`):** Serves as the user-facing delivery tool, featuring pivot tables, formulas, and visual charts.
* **Libraries Used:** `pandas`, `openpyxl` [add any others like xlwings, openpyxl, matplotlib].

---




