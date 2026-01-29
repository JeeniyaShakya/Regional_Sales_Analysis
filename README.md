# Regional Sales & Profitability Performance (2014–2017)

## 📌 Project Overview
This project analyzes the sales performance of a fictional corporation to identify the core drivers of revenue and profitability. By transforming raw transactional data into a high-fidelity, interactive **Power BI dashboard**, this analysis enables leadership to move beyond "gut feeling" and make data-driven decisions regarding regional expansion, product pricing, and channel optimization.

## 🎯 Goal & Purpose
The objective was to create an **Executive-Ready Dashboard** providing both a 30,000-foot strategic view and granular drill-down capabilities:

* **Identify Profitability Drivers:** Pinpoint products and regions maintaining the highest margins, not just high volume.
* **Customer Segmentation:** Analyze the relationship between sales volume and profit margin to identify "High-Value" vs. "Underperforming" customers.
* **Operational Efficiency:** Evaluate sales channel performance (Wholesale vs. Distributor vs. Export) to optimize resource allocation.
* **Seasonal Trend Analysis:** Uncover patterns in monthly sales to assist in inventory and budget planning.

## 📊 Key Visuals & Analysis
The dashboard is strategically split into two primary focus areas:

### 1. Executive Sales Performance
* **Dynamic KPIs:** Real-time tracking of **Total Revenue ($1.19bn)**, **Total Profit ($443.92M)**, and **Profit Margin (37.37%)**.
* **Regional Deep Dive:** Comparison of "Top States by Revenue" (led by California and Illinois) vs. "Top States by Orders" to distinguish between volume-heavy and value-heavy markets.
* **Monthly Sales Trend:** A minimalist time-series chart highlighting seasonal peaks and year-over-year stability.

### 2. Sales Drivers & Profitability Analysis
* **Customer Segmentation Scatter Plot:** A "Revenue vs. Profit Margin" visualization used to segment the customer base into four distinct quadrants for targeted marketing.
* **Average Order Value (AOV) Distribution:** A high-density frequency chart showing where the majority of customer spend occurs.
* **Top 10 Products by Profit:** A targeted bar chart identifying the most profitable individual SKUs to inform pricing strategies.

## 💡 Business Impacts & Insights
* **Risk Mitigation:** Identified a high revenue concentration in California, suggesting a need for market diversification to reduce regional risk.
* **Channel Optimization:** Determined that while **Wholesale** drives the majority of volume (54%), the **Export** channel provides critical margin support.
* **Product Strategy:** Focusing promotions on high-yield "Top 10" products rather than low-margin volume drivers to maximize bottom-line growth.

## 📸 Screenshots of Dashboard
| Page 1: Executive Overview | Page 2: Drivers & Profitability |
| :--- | :--- |
| ![Executive Performance](https://github.com/JeeniyaShakya/Regional_Sales_Analysis/blob/main/Screenshot%202026-01-29%20162705.png) | ![Profitability Analysis](https://github.com/JeeniyaShakya/Regional_Sales_Analysis/blob/main/Screenshot%202026-01-29%20162727.png) |

## 🛠️ Techniques Used
The project followed a standard data analytics workflow combining **Python** for data engineering and **Power BI** for business intelligence:

* **Business Understanding:** Defining the core problem statement and business objectives for the 2014-2017 period.
* **Data Preparation & Cleaning (Python/Power Query):**
    * Merged multiple relational Excel sheets (Sales Orders, Customers, Products, Regions, States, and Budgets).
    * Standardized headers, handled null values, and converted column names to lowercase for consistency.
    * Removed redundant columns based on domain knowledge.
* **Exploratory Data Analysis (EDA):** Leveraged **Pandas, NumPy, Matplotlib, and Seaborn** for initial data inspection and descriptive statistics.
* **Advanced Data Modeling (DAX):** Created complex weighted average measures (e.g., `Profit Margin %` and `Avg Profit Margin per Product`) to ensure accurate aggregation across different dimensions.
* **Interactive Dashboarding:** Developed a multi-page interactive report featuring dynamic slicing, cross-filtering, and a cohesive UI/UX.

---

### How to use
1. Clone the repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. (Optional) Review the `eda_notebook.ipynb` for the initial Python data cleaning process.
