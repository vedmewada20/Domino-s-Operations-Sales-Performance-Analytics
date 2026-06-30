# Domino's-Operations-Sales-Performance-Analytics

## 📌 Project Overview
This repository showcases an end-to-end data analytics solution designed to evaluate sales performance, optimize delivery operations, and uncover actionable consumer insights using a dataset of over 50,000 operational records from Domino's. 

The project spans the entire data lifecycle: **Data Cleaning & Wrangling** via Python, **Exploratory Data Analysis (EDA)**, and **Interactive Dashboard Engineering** using Power BI to translate complex raw metrics into strategic business decisions.

---

## 🛠️ Tech Stack & Toolkit
* **Data Processing & Engineering:** Python, Pandas, NumPy
* **Environment:** Jupyter Notebook
* **Business Intelligence & Visualization:** Power BI Desktop (DAX, Power Query)
* **Dataset Source:** Kaggle (Simulated 50,000+ transactional records)

---

## ⚙️ Data Pipeline & Cleaning Process
The initial raw dataset (`dominoz_unclean_50k.csv`) presented significant real-world challenges, including missing values, incorrect data types, and logical inconsistencies. The processing notebook (`dominoz_data (2).ipynb`) executed the following pipeline:

1. **Handling Structural Inconsistencies:** Standardized mixed-case strings across categorical fields like `pizza_variant`, `order_type`, and `payment_method`.
2. **Missing Data Imputation:** Formulated logic to handle null values in critical operational categories like `order_status` and `special_request`.
3. **Feature Engineering:** * Extracted time-based dimensions (`order_hour`, `order_day`, `order_month`) to uncover peak operational windows.
    * Calculated metrics to isolate true delivery durations and flag extreme anomalies.
4. **Export:** Delivered a verified, analytics-ready dataset (`dominoz_clean_final.csv`) for business intelligence mapping.

---

## 📊 Power BI Dashboard Features
The interactive dashboard (`dominos.pbix`) acts as a strategic control tower for regional managers. Key components include:

* **Sales & Revenue Engine:** Visualizes total revenue, quantity sold, and average order value segmented by pizza variants (e.g., Margherita, Pepperoni, Veggie, Paneer Tikka).
* **Operational Efficiency Trackers:** Measures delivery performance across multiple store locations (`store_1` through `store_4`) by crossing delivery distance against duration.
* **Customer Preferences:** Analyzes correlations between payment methods (UPI, Cash, Cards), coupon usage, and final customer ratings.
* **Dynamic Granular Control:** Fully equipped with interactive slicers for time periods, store IDs, and payment options to allow targeted drill-downs.

---

## 📈 Key Business Insights Uncovered
* **Peak Demand Windows:** Clear revenue spikes identified during specific hours and weekend cycles, highlighting clear scheduling optimization opportunities for store staff.
* **Delivery Logistics Bottlenecks:** Cross-referencing distance versus duration highlighted specific stores encountering logistics friction, enabling targeted localized operational updates.
* **Transaction Drivers:** UPI and Cash dominate payment shares; mapping these against coupon usage reveals clear avenues for targeted loyalty program placements.

---

## 📁 Repository Structure

├── canvas_dominos.png         # UI Wireframe / Dashboard Design Canvas
├── domi_canvas.png            # Dashboard Component Layout Plan
├── dominoz_data (2).ipynb     # Python Jupyter Notebook for Data Cleaning & EDA
├── dominoz_unclean_50k.csv    # Raw, unprocessed initial dataset
├── dominoz_clean_final.csv    # Cleaned, engineered final dataset utilized in BI
├── dominos.pbix               # Complete Power BI Dashboard File
└── README.md                  # Project Documentation

## Project Files 
text[dominoz_clean_final.xlsx](https://github.com/user-attachments/files/29500838/dominoz_clean_final.xlsx)

[dominoz_unclean_50k.csv](https://github.com/user-attachments/files/29500850/dominoz_unclean_50k.csv)

[dominoz_data (2).ipynb](https://github.com/user-attachments/files/29500849/dominoz_data.2.ipynb)
