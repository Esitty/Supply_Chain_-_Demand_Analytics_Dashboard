# Supply Chain & Demand Analytics Dashboard

An Excel dashboard analyzing product demand, inventory management, and supplier performance across warehouse locations in Germany, built to identify supply chain inefficiencies and support operational decision-making.

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Pivot Tables](https://img.shields.io/badge/Pivot_Tables_%26_Charts-217346?style=flat)
![Supply Chain](https://img.shields.io/badge/Supply_Chain_Analytics-7B2D8B?style=flat)

---

## 🎯 Business Problem

Companies managing multi-product distribution across multiple warehouses routinely struggle to connect four operational threads in a single view:

- Are we ordering and delivering the right quantities relative to actual demand?
- Which products are consistently overstocked, and what is that costing us?
- Which suppliers are reliable, and which are creating delivery risk?
- Are our most profitable products the ones we are prioritising operationally?

This project addresses those questions by building a unified dashboard that links product performance, inventory gaps, and supplier behaviour enabling managers to make faster, evidence-based decisions across procurement, warehouse, and sales functions.

---

## 📊 Key Performance Indicators

| Metric | Value |
|---|---|
| Total Revenue | €1,349,500 |
| Total Units Sold | 2,970 |
| Average Delivery Time | 6.1 days |
| Overall Profit Margin | 31.57% |

---

📸 Dashboard Preview

<img width="561" height="910" alt="Supply Chain   Demand" src="https://github.com/user-attachments/assets/a8fab5cb-be36-4e68-8959-a7d0d68f15ce" />

---

## 🔧 My Process

**1 — Data cleaning & structuring**
Standardized product type categories, validated units ordered vs. units delivered vs. units sold for consistency, checked for anomalies in delivery time records, and confirmed revenue and cost figures balanced correctly across all four product lines and three suppliers.

**2 — Defining the analytical framework**
Identified five core analytical questions before building any charts: product revenue & profit, demand vs. supply balance, inventory gap by product, supplier delivery volume, and supplier delivery speed. Each chart in the dashboard answers exactly one of these questions.

**3 — Inventory gap calculation**
Created a calculated field: Inventory Gap = Units Delivered − Units Sold. A positive gap indicates overstocking. Surfaced this per product to identify where excess inventory is accumulating and where it is most severe.

**4 — Supplier performance analysis**
Built two separate supplier views, total units delivered (volume reliability) and average delivery time (speed reliability) because a supplier can be high-volume but slow, or fast but low-volume. Separating these surfaces nuance that a combined metric would hide.

**5 — Slicer & filter design**
Connected Product Type, Supplier, and Warehouse Location slicers to all charts simultaneously, allowing the dashboard to answer location specific or supplier-specific questions without rebuilding any views.

**6 — Insights & recommendations panel**
Added a dedicated insights box directly within the dashboard file — so any stakeholder opening it immediately sees the key takeaways without needing to interpret the charts independently.

---

## 🔍 Key Findings & Business Implications

### Product Performance

- **Heat Pumps generate the highest revenue (€420K) despite lower sales volume than Solar Panels.** This is a premium pricing advantage — the business earns more per unit from Heat Pumps than any other product. A Heat Pump stockout costs more revenue per lost sale than any other category, making availability a priority.

- **Solar Panels record the highest sales volume (990 units)**, making them the primary demand driver. High volume at lower unit revenue means margin management is critical — small cost increases per unit have a large aggregate effect at this scale.

- **EV Chargers underperform across all key metrics** — lowest revenue (€230K) and lowest profit (€86K). Before concluding this is a demand problem, pricing relative to the market and warehouse stocking locations should be examined.

### Inventory Management

- **All four product categories show positive inventory gaps** — more units are delivered than sold across the board. This is consistent overstocking, not a one-off. Solar Panels (gap of 155 units) and Batteries (141 units) carry the largest excess. Overstocking ties up working capital and increases warehousing costs; a review of order quantities against actual sales velocity is recommended.

### Supplier Performance

- **Supplier A delivers the highest volume (1,396 units) and fastest average delivery time (3.5 days)** — the strongest overall supplier by both measures. Should be prioritised in procurement negotiations.

- **Supplier C averages 8.7 days delivery time — more than double Supplier A.** At a 6.1-day company average, Supplier C is pulling the mean up significantly. For time-sensitive products like Heat Pumps, reliance on Supplier C creates material delivery risk. Contracts and alternative sourcing should be reviewed.

---

## 📋 Dashboard Features

| Chart / View | Business Question Answered |
|---|---|
| Product performance: revenue, profit & sales volume | Which products generate the most value, and is volume aligned with revenue? |
| Demand vs. supply by product | Are we delivering more than we sell, and by how much? |
| Inventory gap by product | Where is overstocking concentrated? |
| Units delivered by supplier | Which supplier handles the most volume? |
| Average delivery time by supplier | Which supplier is creating delivery risk? |
| KPI summary cards | What is the overall health of the operation at a glance? |
| Insights & recommendations panel | What should a decision-maker act on immediately? |

---

## 🛠 Tools & Techniques

| Tool / Technique | How It Was Used |
|---|---|
| Microsoft Excel | Primary analysis and dashboard environment |
| Pivot Tables | Aggregating revenue, profit, units sold, units delivered, and delivery time by product, supplier, and warehouse location |
| Pivot Charts | Clustered bar charts for demand vs. supply, horizontal bars for supplier comparison, combined bar + line for product performance |
| Slicers | Interactive filtering by Product Type, Supplier, and Warehouse Location across all charts simultaneously |
| Calculated Fields | Inventory gap (units delivered − units sold), profit margin (profit ÷ revenue), average delivery time per supplier |
| KPI Cards | Summary metrics designed for executive-level readability at the top of the dashboard |
| Dashboard Insights Panel | Embedded recommendations box surfacing key findings directly within the dashboard file |

---

## 📁 Dataset Description

| Column | Description |
|---|---|
| Date | Transaction date |
| Product_Type | Battery, EV Charger, Heat Pump, Solar Panel |
| Supplier | Supplier A, B, or C |
| Warehouse_Location | Berlin, Cologne, Frankfurt, Hamburg, Munich |
| Units_Ordered | Quantity ordered from supplier |
| Units_Delivered | Quantity actually received |
| Units_Sold | Quantity sold to end customers |
| Delivery_Time | Days between order and delivery |
| Revenue | Total sales revenue (€) |
| Cost | Total procurement cost (€) |
| Profit | Revenue minus cost (€) |

---

## 💼 Transferable Skills Demonstrated

- Supply chain analysis - demand planning, inventory control, and supplier evaluation applicable across manufacturing, retail, logistics, and energy sectors
- Structuring a multi-dimensional analysis (product + supplier + location) into a single coherent dashboard
- Translating operational metrics into business language that non-technical stakeholders can act on
- Identifying where operational inefficiency is creating financial cost not just describing what the data shows
- Designing dashboards that serve multiple functions simultaneously: performance review, risk identification, and procurement planning

---

*Dataset is simulated to reflect real-world supply chain operations.*
