# 📊 Customer Analysis Dashboard — Tableau

An interactive **Customer Analysis Dashboard** built using **Tableau** to analyze sales performance, customer behavior, revenue distribution, demographics, geography, and discount patterns.

The project uses one year of transactional sales data and transforms it into a set of interactive visualizations that provide insights into **revenue trends, customer segments, product categories, geographic performance, and purchasing patterns**.

---

## 📌 Project Overview

The objective of this project is to explore customer and sales data from **October 2020 to September 2021** and answer questions such as:

* How much revenue was generated?
* Which product categories contribute the most revenue?
* How does revenue vary across months?
* Which regions and states generate the highest revenue?
* How does customer age relate to revenue?
* Is there a relationship between quantity purchased and discount percentage?
* How does revenue vary between male and female customers?
* Which payment methods are most commonly associated with purchases?

The final result is an interactive Tableau dashboard that brings these different perspectives together in a single view.

---

## 🛠️ Tools & Technologies

* **Tableau** — Data visualization and dashboard development
* **CSV** — Source data
* **Data Cleaning & Preparation** — Preparation of transactional and customer attributes
* **Calculated Fields / Bins** — Used for demographic analysis
* **Interactive Dashboarding** — Combining multiple visualizations into a single analytical view

---

## 📂 Dataset

The dataset contains transactional sales information along with customer, product, geographic, demographic, and payment-related attributes.

### Dataset Summary

| Attribute              |               Value |
| ---------------------- | ------------------: |
| Time Period            | Oct 2020 – Sep 2021 |
| Total Rows             |             286,392 |
| Unique Orders          |             201,716 |
| Unique Customers       |              64,248 |
| Product Categories     |                  15 |
| States                 |                  51 |
| Regions                |                   4 |
| Total Quantity Ordered |             862,411 |
| Gross Value            |            ~253.71M |
| Discount Amount        |             ~20.06M |
| Total Revenue          |            ~233.65M |

### Important Dataset Fields

#### Transaction Information

* `order_id` — Unique order identifier
* `order_date` — Date of the order
* `status` — Order status
* `item_id` — Item identifier
* `sku` — Product SKU
* `qty_ordered` — Quantity ordered
* `price` — Product price
* `value` — Order/item value
* `discount_amount` — Discount applied
* `total` — Final transaction amount

#### Product Information

* `category` — Product category
* `payment_method` — Payment method
* `bi_st` — Business/order status indicator

#### Customer Information

* `cust_id` — Customer identifier
* `Gender` — Customer gender
* `age` — Customer age
* `Customer Since` — Customer registration/start date
* `full_name` — Customer name
* `E Mail` — Customer email
* `User Name` — Customer username

#### Geographic Information

* `Place Name`
* `County`
* `City`
* `State`
* `Zip`
* `Region`

#### Other Fields

* `year`
* `month`
* `ref_num`
* `Discount_Percent`

---

# 📊 Dashboard

The dashboard is titled **Customer Analysis** and combines multiple visualizations to provide a comprehensive overview of sales and customer behavior.

The dashboard contains the following views:

1. Total Revenue
2. Revenue per Month
3. Revenue per Category per Gender
4. Revenue per State
5. Revenue per Region
6. Revenue Based on Age
7. Quantity–Discount Percentage Correlation

---

## 💰 1. Total Revenue

The dashboard provides an overall revenue KPI representing the total transaction value.

Based on the supplied dataset:

**Total Revenue ≈ 233.65M**

The dashboard uses the `total` field as the primary revenue metric.

This KPI provides a high-level snapshot of the overall sales performance during the analyzed period.

---

## 📅 2. Revenue per Month

The monthly revenue visualization analyzes how sales changed throughout the year.

### Key Observation

December 2020 generated the highest revenue, with approximately:

**57.67M**

Other strong months included:

* April 2021 — ~36.70M
* March 2021 — ~25.16M
* June 2021 — ~24.65M

The lowest revenue was recorded in:

* February 2021 — ~4.40M
* October 2020 — ~5.30M

This visualization can help identify:

* Seasonal purchasing patterns
* High-performing months
* Low-demand periods
* Potential promotional opportunities
* Changes in customer purchasing behavior over time

---

## 🛍️ 3. Revenue per Category per Gender

This visualization examines revenue across product categories while breaking the results down by gender.

The dataset contains **15 product categories**, including:

* Mobiles & Tablets
* Appliances
* Entertainment
* Others
* Computing
* Women's Fashion
* Men's Fashion
* Superstore
* Beauty & Grooming
* Home & Living
* Health & Sports
* Kids & Baby
* Soghaat
* School & Education
* Books

### Category Performance

The highest-revenue category is:

**Mobiles & Tablets — ~130.11M**

It is followed by:

**Appliances — ~30.06M**

and

**Entertainment — ~27.14M**

Mobiles & Tablets therefore represents a particularly significant portion of overall revenue.

The gender breakdown allows the business to investigate whether particular categories perform differently across customer segments.

---

## 🌎 4. Revenue per Region

The dashboard also evaluates revenue geographically using four major regions:

* South
* Midwest
* West
* Northeast

### Regional Performance

| Region    | Revenue |
| --------- | ------: |
| South     | ~89.65M |
| Midwest   | ~62.92M |
| West      | ~41.12M |
| Northeast | ~40.00M |

The **South region** generated the highest revenue in the dataset.

Geographic analysis can help identify:

* High-performing markets
* Regions requiring additional marketing
* Regional sales opportunities
* Differences in customer demand

---

## 🗺️ 5. Revenue per State

The state-level visualization provides a more granular geographic analysis of revenue.

Some of the highest-revenue states include:

| State        | Approx. Revenue |
| ------------ | --------------: |
| Texas        |         ~15.47M |
| California   |         ~13.88M |
| New York     |         ~11.37M |
| Pennsylvania |         ~10.16M |
| Illinois     |          ~9.11M |
| Florida      |          ~8.46M |
| Virginia     |          ~8.19M |
| Ohio         |          ~8.15M |
| Missouri     |          ~8.00M |
| Kentucky     |          ~6.99M |

This visualization makes it easier to identify geographic concentration in sales and compare individual state performance.

---

## 👥 6. Revenue Based on Age

Customer age is analyzed using an **age bin**, allowing customers to be grouped into age ranges instead of analyzing every individual age separately.

This helps answer questions such as:

* Which age groups generate the most revenue?
* Are younger or older customers more valuable?
* Are there specific demographic segments with higher purchasing activity?

The age-based visualization can support customer segmentation and targeted marketing strategies.

---

## 🏷️ 7. Quantity–Discount Percentage Correlation

The dashboard includes a visualization examining the relationship between:

* `qty_ordered`
* `Discount_Percent`

The purpose is to investigate whether larger quantities are associated with higher discounts.

Potential business questions include:

* Do customers purchase more when discounts increase?
* Are larger orders receiving larger discounts?
* Is there evidence of volume-based purchasing behavior?
* Could discount strategies be influencing order quantities?

This visualization provides a starting point for investigating the relationship between pricing incentives and customer purchasing behavior.

---

# 🔍 Key Insights

Based on the supplied dataset, several important patterns emerge.

### 1. Mobile & Tablet Sales Dominate

**Mobiles & Tablets** generated approximately **130.11M**, making it the dominant product category in terms of revenue.

This indicates that electronics/mobile-related products represent a major revenue driver.

### 2. December Was the Strongest Month

December 2020 generated approximately **57.67M**, substantially higher than most other months.

This may indicate strong seasonal demand or promotional activity around the end of the year.

### 3. The South Is the Strongest Region

The South generated approximately **89.65M**, making it the highest-revenue region among the four geographic regions.

### 4. Revenue Is Relatively Balanced by Gender

Revenue between the two gender groups was very similar:

* Female: ~116.65M
* Male: ~117.00M

This suggests that overall revenue is not heavily concentrated in one gender segment.

### 5. Texas Is the Highest-Revenue State

Texas generated approximately **15.47M**, followed by California at approximately **13.88M**.

This highlights Texas as one of the most important individual markets in the dataset.

---

# 📈 Dashboard Design

The dashboard combines multiple perspectives rather than relying on a single visualization.

### Analytical Dimensions

The dashboard analyzes sales from several dimensions:

**Time**

* Month
* Year
* Order Date

**Customer**

* Gender
* Age
* Customer ID

**Product**

* Category
* SKU
* Item

**Geography**

* Region
* State
* City

**Transaction**

* Quantity
* Revenue
* Discount
* Payment Method
* Order Status

This multidimensional approach allows users to move from a high-level revenue overview to more detailed customer and transaction-level analysis.

---

# 🧮 Calculated Fields & Data Preparation

The Tableau workbook uses an **Age Bin** calculated field to group customers into age ranges.

The workbook also uses the existing transactional fields to construct the different visualizations.

The primary revenue measure used throughout the dashboard is:

```text
SUM(total)
```

Other important measures include:

```text
SUM(qty_ordered)
SUM(value)
SUM(discount_amount)
```

Dimensions such as category, gender, region, state, month, and age are used to break down these measures.

---

# 📊 Tableau Worksheets

The workbook contains the following worksheets:

| Worksheet                                | Purpose                        |
| ---------------------------------------- | ------------------------------ |
| Total revenue                            | Overall revenue KPI            |
| Revenue per month                        | Monthly revenue trend          |
| Revenue per catagorie per gender         | Category and gender comparison |
| Revenue per state                        | State-level revenue analysis   |
| Revenue per region                       | Regional revenue analysis      |
| Revenue based on age                     | Age-group revenue analysis     |
| Quantity-Discount percentage correlation | Quantity vs. discount analysis |

These worksheets are combined into the **Customer Analysis** dashboard.

---

# 💡 Business Applications

The analysis can potentially help businesses with:

### Customer Segmentation

Identify high-value customer demographics based on age, gender, geography, and purchasing behavior.

### Marketing Strategy

Target high-performing regions, states, categories, and customer segments.

### Product Strategy

Identify categories responsible for the largest share of revenue.

### Pricing & Promotions

Analyze the relationship between discounts and purchasing quantity.

### Seasonal Planning

Use monthly revenue trends to identify periods of high and low demand.

### Geographic Expansion

Identify strong markets and areas with potential for further growth.

---

# ⚠️ Data Privacy Consideration

The original dataset contains sensitive personally identifiable information (PII), including fields such as:

* Email addresses
* Phone numbers
* SSNs
* Customer names
* Usernames
* ZIP codes

**The raw dataset should not be publicly uploaded to GitHub in its original form.**

For a public repository, it is recommended to:

1. Remove sensitive columns.
2. Anonymize customer identifiers.
3. Upload only the columns required for visualization.
4. Add the original CSV to `.gitignore` if it is stored locally.

Example `.gitignore` entry:

```gitignore
sales_06_FY2020-21 copy.csv
```

A sanitized sample dataset can instead be provided for reproducibility.

---

# 🚀 How to Use the Project

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <repository-name>
```

### 2. Open the Tableau Workbook

Open:

```text
Customer analysis.twb
```

using Tableau Desktop.

### 3. Connect the Dataset

If Tableau cannot locate the source CSV, update the data source path to point to the sanitized dataset.

### 4. Explore the Dashboard

Use the dashboard to analyze:

* Revenue trends
* Customer demographics
* Product categories
* Gender-based purchasing
* Regional performance
* State-level performance
* Age-group performance
* Discount behavior

---

# 🎯 Project Objective

The main objective of this project is to demonstrate how **Tableau can be used to transform raw transactional data into an interactive business intelligence dashboard**.

The project demonstrates skills in:

* Data exploration
* Data visualization
* Dashboard design
* Customer analysis
* Sales analysis
* Geographic analysis
* Demographic analysis
* KPI development
* Interactive business intelligence
* Analytical storytelling

---

# 📌 Future Improvements

Potential extensions to this project include:

* Customer **RFM (Recency, Frequency, Monetary) analysis**
* Customer lifetime value analysis
* Customer retention and churn analysis
* New vs. returning customer analysis
* Profit and margin analysis
* Product-level performance analysis
* Sales forecasting
* Interactive filters for category, region, gender, and customer segment
* Drill-down from region → state → city
* Advanced discount elasticity analysis
* Customer segmentation using clustering

---

# 👨‍💻 Author

**Rahul Shah** **IIT Delhi MnC**

This project was created as part of a portfolio of **Data Analytics, Business Intelligence, and Data Visualization projects**.

---

## ⭐ If You Found This Project Useful

If you found this project interesting, consider giving the repository a ⭐ and exploring the Tableau workbook to interact with the dashboard.
