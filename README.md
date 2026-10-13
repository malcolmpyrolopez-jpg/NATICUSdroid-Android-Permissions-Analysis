# NATICUSdroid-Android-Permissions-Analysis
An exploratory data analysis and Power BI visualization project analyzing 29,000+ benign and malicious Android applications to identify permission abuse patterns and security risks.
# NATICUSdroid: Android Permission Malware Analysis & Visualization

An exploratory data analysis project examining permission patterns across more than 29,000 benign and malicious Android applications released between 2010 and 2019. This project leverages Power BI and SQL-based insights to highlight security risks, permission abuse, and high-risk indicators for malware detection[cite: .

##  Project Overview
Mobile malware often relies on exploiting specific Android system permissions. This project analyzes the **NATICUSdroid dataset** to uncover behavioral differences between legitimate apps and malware, focusing on which requested permissions pose the highest security risks.

### Key Objectives:
* **Identify Risky Permissions:** Determine which permissions have the highest association with malicious applications.
* **Comparative Analysis:** Contrast permission usage frequencies between benign and malicious apps.
* **Data Visualization:** Transform raw permission data into actionable visual insights for security assessment and monitoring.

---

##  Key Findings & Insights
* **High-Risk Permissions:** Permissions related to **phone state**, **location access**, and **boot reception (`RECEIVE_BOOT_COMPLETED`)** demonstrated the highest malicious usage ratios, marking them as critical risk indicators.
* **Functional vs. Misused Permissions:** While broad functional permissions (such as `INTERNET` and `ACCESS_NETWORK_STATE`) are commonly requested by both benign and malicious apps, their usage frequency distributions help highlight potential abuse patterns.
* **Ecosystem Trends:** Most Android applications rely on internet connectivity for core features, while fewer apps request sensitive permissions like location and device states.

---

##  Tools & Technologies
* **Data Source:** [NATICUSdroid Dataset (UCI Machine Learning Repository)](https://archive.ics.uci.edu/dataset/722/naticusdroid+android+permissions+dataset)
* **Data Processing & Querying:** SQL
* **Data Visualization:** Power BI

---

##  Project Structure & Usage
1. **Data Cleaning & Transformation:** Cleaned raw application permission logs to isolate binary classification results (Benign vs. Malicious).
2. **SQL Analysis:** Executed aggregate queries to evaluate permission distribution and app classification counts.
3. **Power BI Dashboards:** Built visual reports showcasing top requested permissions, risky permission ratios, and comparative frequency charts.
