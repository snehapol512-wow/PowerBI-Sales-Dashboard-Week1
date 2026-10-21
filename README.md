# Power BI Week 1 Project: Sales Performance Dashboard

## 📌 Executive Summary & Project Requirements
This dashboard fulfills all the requirements specified in **Week 1: Introduction to Power BI & Data Modelling**:
1. **Total Revenue**: Comprehensive KPI tracking overall sales revenue ($118.73M).
2. **Sales by Region**: Regional comparison visual breaking down revenue across all 5 countries.
3. **Top 5 Products by Profit**: Profitability analysis ranking the top 5 most profitable products.
4. **Interactive Filters**: Dynamic year slicers (2013, 2014) and customer segment slicers.

---

## 📊 Key Business Metrics Summary
- **Total Revenue (Sales)**: **$118,726,350.26** (~$118.73M)
- **Total Gross Sales**: **$127,931,598.50** (~$127.93M)
- **Total Net Profit**: **$16,893,702.26** (~$16.89M)
- **Total Units Sold**: **1,125,806 units** (~1.13M)
- **Overall Profit Margin**: **14.23%**

---

## 🌍 Sales by Region (Country Breakdown)
| Rank | Country / Region | Total Revenue (Sales) | % Share of Total Sales |
| :--- | :--- | :--- | :--- |
| **1** | **United States of America** | $25,029,830.17 | 21.08% |
| **2** | **Canada** | $24,887,654.88 | 20.96% |
| **3** | **France** | $24,354,172.28 | 20.51% |
| **4** | **Germany** | $23,505,340.82 | 19.80% |
| **5** | **Mexico** | $20,949,352.11 | 17.65% |
| **Total** | **All Regions** | **$118,726,350.26** | **100.0%** |

---

## 🏆 Top 5 Products by Profit
| Rank | Product | Total Profit | Total Revenue (Sales) | Profit Margin |
| :--- | :--- | :--- | :--- | :--- |
| **1** | **Paseo** | **$4,797,437.95** | $33,011,143.95 | 14.53% |
| **2** | **VTT** | **$3,034,608.02** | $20,511,921.02 | 14.79% |
| **3** | **Amarilla** | **$2,814,104.06** | $17,747,116.06 | 15.86% |
| **4** | **Velo** | **$2,305,992.46** | $18,250,059.46 | 12.64% |
| **5** | **Montana** | **$2,114,754.88** | $15,390,801.88 | 13.74% |
| *6 (Excluded)* | *Carretera* | *$1,826,804.89* | *$13,815,307.89* | *13.22%* |

---

## 👥 Sales by Customer Segment
- **Government**: $52,504,260.67 (44.22%) — *Primary revenue driver*
- **Small Business**: $42,427,918.50 (35.74%) — *High growth potential*
- **Enterprise**: $19,611,694.38 (16.52%)
- **Midmarket**: $2,381,883.07 (2.01%)
- **Channel Partners**: $1,800,593.64 (1.52%)

---

## 📐 Data Modeling & DAX Measures Used
In Power BI Desktop, the following DAX measures were constructed:

```dax
// 1. Total Revenue Measure
Total Revenue = SUM(financials[Sales])

// 2. Total Gross Sales Measure
Total Gross Sales = SUM(financials[Gross Sales])

// 3. Total Net Profit Measure
Total Profit = SUM(financials[Profit])

// 4. Total Units Sold Measure
Total Units Sold = SUM(financials[Units Sold])

// 5. Profit Margin %
Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)
```

---

## 🔗 How to Submit This Assignment as a Link

You have 3 easy ways to submit this assignment depending on your course/portal requirements:

### Method 1: Google Drive Link (Recommended & Easiest — 30 Seconds)
1. Go to [Google Drive](https://drive.google.com).
2. Click **+ New** > **File upload**.
3. Select `Sales_Dashboard_Week1.pbix` from `Desktop/PowerBI_Sales_Dashboard_Week1`.
4. Once uploaded, right-click the file and click **Share** > **Share**.
5. Under **General access**, switch from "Restricted" to **"Anyone with the link"** (Role: Viewer).
6. Click **Copy link** and paste it into your assignment submission box.

### Method 2: GitHub Repository Link
1. Log in to [GitHub](https://github.com).
2. Create a new repository named `PowerBI-Sales-Dashboard-Week1`.
3. Upload the files in this folder (`Sales_Dashboard_Week1.pbix`, `index.html`, `sample_financial_data.xlsx`, `README.md`).
4. Copy your repository link:
   `https://github.com/snehapol512-wow/PowerBI-Sales-Dashboard-Week1`
5. *(Bonus)* Go to repo **Settings** > **Pages** > Select `main` branch > Click **Save**. Your interactive dashboard will be live at:
   `https://snehapol512-wow.github.io/PowerBI-Sales-Dashboard-Week1/`

### Method 3: Power BI Service "Publish to Web" Link
1. Double-click `Sales_Dashboard_Week1.pbix` on your Desktop to open in Power BI Desktop.
2. In the top ribbon (Home tab), click **Publish**.
3. Select **My Workspace** and click **Select**.
4. When publish is successful, open the report in Power BI Web.
5. Click **File** > **Embed report** > **Publish to web (public)**.
6. Click **Create embed code** > **Publish** > Copy the generated public link (`https://app.powerbi.com/view?r=...`).
