## Charts Visualization Tools

1. Waterfall Chart
2. Gauge Chart
3. Line Chart
4. Line Chart Drill with Slicer
5. Area chart
6. Stack Area Chart
7. Line vs Stacked Column Chart
8. Line vs Clustered Chart
9. Scatter Plot - use numeric value (use animation -  export file)
10. Tree map


### **Waterfall Chart**

A **Waterfall Chart** shows how positive and negative values impact a total over time, helping **visualize increases, decreases, and overall changes in metrics** like **sales** or **profit**.

**Waterfall Chart – Build Setup**
- **Waterfall chart  (Build ) —> Category / Breakdown / Y-axis / Tooltips**
- **Waterfall (Format) —> size and style/ title / x-axis / y-axis / legend / gridlines / columns / breakdown / data labels / plot are background / reference line**


### **Examples**

#### **1. Increase in Data (Sales by Market)**  
**Steps:**  
- Waterfall Chart → **Category:** Market  
- Waterfall Chart → **Y-axis:** Sales  
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

#### **2. Decrease in Data (Sales by Market and Category)**  
**Steps:**  
- Waterfall Chart → **Category:** Market  
- Waterfall Chart → **Y-axis:** Sales  
- Waterfall Chart → **Breakdown:** Category  
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

#### **3. Compare Positive and Negative Values**  
**Steps:**  
- Waterfall Chart → **Category:** Order Date  
- Waterfall Chart → **Y-axis:** Sales  
- Waterfall Chart → **Breakdown:** Category  
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

---

### **Gauge Chart**
A Gauge Chart is used to show **progress toward a target or goal within a defined range**.

**Gauge Chart – Build Setup**
- **Gauge (Build) —> value / min value / max value / target value / tooltips** 
- **Format (Visual) —> size and style / title / gauge axis / colors / data labels / target label / callout value**

**Examples :** To analyze category and sub-category performance against the target shown in the Gauge chart, use a Donut chart and a Slicer.

**Gauge Chart (Sales vs Profit)** Visualize how Sales perform against the Profit target.
- Gauge (Build) —> value (sales)
- Gauge (Build) —> target value (profit)
- Gauge (Format) —> color (fill color —> blue, target color —> red)

**Donut Chart Analysis (Category Performance)** Analyze category-wise and sub-categor performance against targets.

- Donut chart  (Build) —> legend (category)
- Donut chart  (Build) —> value (sales)

**Slicer Setup (Sub-Category Filter)** Filter Donut Chart results by sub-category.

- Slicer (Build)  —> field (sub category)
- Slicer (Format) —>  (title —> on ,  slicer header —>on)
- Slicer (Format) —> slicer setting —> options (style —> dropdown)

---
