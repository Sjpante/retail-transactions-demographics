# Retail Transactions & Customer Demographics Analysis 🛒📊

> **⚠️ Viewing Note:** This project utilizes custom HTML/CSS formatting and interactive Plotly visualizations. If viewing the raw `.ipynb` file in an IDE with a Dark Mode theme (like VS Code) or the native GitHub viewer, some text rendering and formatting may clash. For the optimal viewing experience, please download the repository and open the attached `.html` export directly in a web browser.

## 📌 Project Overview
This project analyzes over 2 million retail transactions to uncover purchasing trends, evaluate promotional efficiency, and identify high-value customer segments based on household demographics. 

By merging daily transaction logs with customer profiles, this analysis transitions from raw data engineering to actionable business insights, culminating in targeted recommendations for marketing and inventory management.

## 🎯 Key Objectives & Business Questions
* **Macro KPIs:** What is the store-wide baseline for Total Sales, Total Discount Rate, and Average Household Spend?
* **Time-Series Trends:** How do sales fluctuate by month and day of the week across 2016 and 2017?
* **Customer Profiling (The "Whales"):** Who are the top 10 households driving top-line revenue, and what is their demographic makeup?
* **Product Efficiency:** Are top-selling items heavily reliant on promotional discounts, or do they drive organic revenue?

## 🛠️ Tools & Techniques
* **Language:** Python 3
* **Environment:** Jupyter Notebook
* **Libraries:** Pandas, NumPy, Plotly Express
* **Techniques Demonstrated:**
  * **Big Data Handling:** Downcasting `int64` and `float64` types to reduce dataset memory footprint by >20%.
  * **Feature Engineering:** Calculating absolute discount values and relative percentage rates from raw transaction logs.
  * **Relational Data Merging:** Utilizing `pd.merge()` and `.query()` to map raw IDs to readable product descriptions and demographic profiles.
  * **Interactive Visualization:** Building custom, styled bar charts and trend lines using Plotly.
  * **Reporting:** Dynamic Pivot Tables and custom Pandas display formatting.

## 💡 Key Insights Discovered
1. **The Pareto Principle in Action:** A very small fraction of households act as "whales," driving a disproportionate amount of total revenue.
2. **Promotional Efficiency:** The store operates at an average 17.68% discount rate, but bulk anomalies (like Gasoline purchases) skew volume metrics without heavily impacting discount margins.
3. **Demographic Power:** Income and household size strongly correlate with transaction frequency and overall customer lifetime value.

## 📂 Repository Structure

* [**Retail_Transactions_and_Demographics.ipynb**](./Retail_Transactions_and_Demographics.ipynb): The main Jupyter Notebook containing all code, analysis, and custom HTML/CSS reports.
* [**Retail_Transactions_and_Demographics.html (Interactive Preview)**](https://htmlpreview.github.io/?https://github.com/Sjpante/retail-transactions-demographics/blob/main/Retail_Transactions_and_Demographics.html): Click here to view the full interactive report with Plotly charts directly in your browser.
* [**2016-2017_comparison.png**](./2016-2017_comparison.png): Sample Plotly visualization exported from the analysis.

* ## 💾 Data Source
Due to GitHub's file size limits, the raw transaction datasets (2M+ rows) are hosted externally. 

* **To replicate this analysis:** You can download the original CSV files from this **[Google Drive Folder](https://drive.google.com/drive/folders/1I0Qg59rTjymzFpQNPnA246Ve9erYCe7q?usp=sharing)**.
* Save the downloaded `.csv` files into a local folder on your machine and update the file paths in the first cell of the Jupyter Notebook to run the code.
