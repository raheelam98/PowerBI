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

**Notes**

- Tooltips :- Line and Stacked Column chart (Build) —> tooltip (sub category)
Shows sub category in tables
  - Tooltip —> (right click) Data —> Summarization (sum / average / min / max / count / sd / variance / median )
- Export data :-Send selected data to the client in of excel or cvs files

**Format**
- Title :- top (name )
- Legend :- labels
- Detail labels :-   data values
- **Format → Lines** → Apply setting to / Line / Color / Reset to default  
- **Format → Markers** → Apply setting / Shape / Color / Border / Reset to default
  - (Format) —> Markers —> Shape ( type —> dash) remove the shape
  -  Markers : change shape and color of markers
-  


---

### **Waterfall Chart - 1**

A **Waterfall Chart** shows how positive and negative values impact a total over time, helping **visualize increases, decreases, and overall changes in metrics** like **sales** or **profit**.

**Waterfall Chart – Build Setup**
- **Waterfall chart  (Build )** —> Category / Breakdown / Y-axis / Tooltips
- **Waterfall (Format)** —> size and style/ title / x-axis / y-axis / legend / gridlines / columns / breakdown / data labels / plot are background / reference line


### **Examples**

**1. Increase in Data (Sales by Market)**   
- **Waterfall Chart**
  - **Category:** Market  
  - **Y-axis:** Sales  
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

**2. Decrease in Data (Sales by Market and Category)**  
- **Waterfall Chart**
  - **Category:** Market  
  - **Y-axis:** Sales
  - **Breakdown:** Category 
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

**3. Compare Positive and Negative Values**  
- **Waterfall Chart**
  - **Category:** Order Date   
  - **Y-axis:** Sales
  - **Breakdown:** Category
- **Format:** Turn *Title*, *Legend*, and *Data Labels* **On**

---

### **Gauge Chart - 2**
A Gauge Chart is used to show **progress toward a target or goal within a defined range**.

**Gauge Chart – Build Setup**
- **Gauge (Build)** —> value / min value / max value / target value / tooltips 
- **Format (Visual)** —> size and style / title / gauge axis / colors / data labels / target label / callout value

**Examples :** To analyze category and sub-category performance against the target shown in the Gauge chart, use a Donut chart and a Slicer.

**Gauge Chart (Sales vs Profit)** Visualize how Sales perform against the Profit target.
- **Gauge** (Build)
  - value (sales)
  - target value (profit)
- Gauge (Format) —> color (fill color —> blue, target color —> red)

**Donut Chart Analysis (Category Performance)** Analyze category-wise and sub-categor performance against targets.

- **Donut chart**  (Build) 
  - legend (category)
  - value (sales)

**Slicer Setup (Sub-Category Filter)** Filter Donut Chart results by sub-category.

- Slicer (Build)  —> field (sub category)
- Slicer (Format) —>  (title —> on ,  slicer header —>on)
- Slicer (Format) —> slicer setting —> options (style —> dropdown)

---
--- 

### **Line Chart - 3**
Used to show trends over time for one or more categories.

- **Line Chart (Build)** → X-axis / Y-axis / Secondary-axis / Legend / Small multiples / Tooltips  
- **Line Chart (Format)** → Size and style / Title / X-axis / Y-axis / Secondary Y-axis / Legend / Small multiples / Gridlines / Zoom slider / Lines / Shade / Markers / Data labels / Plot area background / Trend line / Reference line / Error bars / Anomalies  

**Note:**  
Avoid using values with too many lines.  
Example — **Legend: Sub-category** (Use a **Column Chart** instead)

**Example 1**  
- **Line Chart**
  - **X-axis:** Order Date  
  - **Y-axis:** Sales  
  - **Legend:** Category 
- Format → Lines → Apply setting to (Furniture)
- Format → Lines → line  
  - Line Style → Dotted  
  - Join Type → Bevel  
  - Interpolation Type → Step  
  - Color → Blue  

**Example 2**
- **Line Chart**
  - **X-axis:** Order Date  
  - **Y-axis:** Region  
  - **Legend:** Category   

- Format → **Lines** → Apply setting to (Furniture)
- Format → Lines → line   
    - Line Style → Dotted  
    - Join Type → Bevel  
    - Interpolation Type → Step  
    - Color → Blue  
- Format → **Markers** → Apply setting  
    - Shape → Type: Dot  

---

### **Line Chart Drill with Slicer - 4**
Used to compare data across multiple years using drill-down.

**Example**
Compare data of **1 and 4 January** for **2013 and 2014**  
*(Data is complex; not recommended for final reports.)*

- **Line Chart**
  - **X-axis:** Order Date  
  - **Y-axis:** Sales  
  - **Legend:** Category
   
  **Slicer** → Field : Order Date  
  - Right Click → Data → Date Hierarchy  
- Format → Slicer Settings → Option → Style → Vertical Line

**Slicer**
- Slicer (Build) → Field: Order Date.
  - Right Click → Data → Date Hierarchy.
- Format → Slicer Settings → Option: Style → Vertical Line.

---

### **Area Chart - 5**
Shows how a single metric changes over time.  
Focuses on **overall trend** (e.g., Total Sales over months).

- **Area Chart (Build)** → X-axis / Y-axis / Secondary-axis / Legend / Small multiples / Tooltips  
- **Area Chart (Format)** → Size and style / Title / X-axis / Y-axis / Secondary Y-axis / Legend / Small multiples / Gridlines / Zoom slider / Lines / Shade / Markers / Data labels / Plot area background / Trend line / Reference line  

**Example 1**  
- **Area Chart**
  - **X-axis:** Order Date  
  - **Y-axis:** Sales  
  - **Legend:** Category  
- Format → Turn *Legend*, *Shade Area* and *Data Labels* **On**
- Format → Markers → Apply settings to → Show for all series → On  
- Format → Markers → Shape → Type: Dot  

---

### **Stacked Area Chart - 6**
Shows how multiple categories contribute to a total over time.  
Useful for comparing **parts to the whole** (e.g., Sales by Region).

**Key Difference:**  
- **Area Chart:** Displays a single trend.  
- **Stacked Area Chart:** Displays multiple stacked trends to show contribution.

- **Stacked Area Chart (Build)** → X-axis / Y-axis / Secondary-axis / Legend / Small multiples / Tooltips  
- **Stacked Area Chart (Format)** → Size and style / Title / X-axis / Y-axis / Legend / Small multiples / Gridlines / Zoom slider / Lines / Shade Area / Markers / Data labels / Series labels / Plot area background / Reference line  

**Example 1**  
*(Convert Order Date to Hierarchy — not a single date field)*  
- **Stacked Area Chart**
-   **X-axis:** Order Date  
-   **Y-axis:** Sales  
-   **Legend:** Category  
- Right-click on Date Column → Data →  
  - Date → Date Column / Date Hierarchy  

---

### **Line vs Stacked Column Chart - 7**
Compares one category across different years (e.g., Compare 2012 vs 2015).

- **Line and Stacked Column Chart (Build)** → X-axis / Column Y-axis / Line Y-axis / Column Legend / Small multiples / Tooltips  
- **Line and Stacked Column Chart (Format)** → Size and style / Title / X-axis / Y-axis / Legend / Small multiples / Gridlines / Zoom slider / Lines / Shade area / Markers / Data labels / Series labels / Plot area background / Reference line  

**Example 1**  Compare one category across years (e.g., 2012–2015)  
- **Line and Stacked Column Chart**
  -  **X-axis:** Order Date  
  - **Column Y-axis** → Category  
  - **Line Y-axis** → Profit  
  - **Column Legend** → Category  
- Format → Turn  **On**  *Title*, *Legend*, *Zoom Slider*, *Marker*, and *Data Labels* 

**Slicer** → Field → Category  

**Example 2 (Small Multiples by Category)**  
- **Line and Stacked Column Chart**
  - **X-axis:** Order Date  
  - **Line Y-axis** → Profit  
  - **Small Multiple** → Category  
- Format → Turn *Title*, *Legend*, *Zoom Slider*, *Marker*, and *Data Labels* **On**

**Slicer** → Field →  Category, Sub-category  

**Note:**  
Sub-category details are not visible in table.  

---

### **Line vs Clustered Column Chart - 8**
Used to compare different categories within the same year.

- **Line and Clustered Column Chart (Build)** → X-axis / Column Y-axis / Line Y-axis / Column Legend / Small multiples / Tooltips  
- **Line and Clustered Column Chart (Format)** → Size and style / Title / X-axis / Y-axis / Legend / Small multiples / Gridlines / Zoom slider / Lines / Shade area / Markers / Data labels / Series labels / Plot area background / Reference line  

**Example 1**  
Compare one category within the same year.  
- **Line and Clustered Column Chart** →
  - **X-axis:** Order Date  
  - **Column Y-axis** → Category  
  - **Line Y-axis** → Profit  
  - **Column Legend** → Category  
  - **Tooltip** → Sub-category  
- Format → Turn *Title*, *Legend*, *Zoom Slider*, *Marker*, and *Data Labels* **On**  

**Slicer** → Field → Category, Sub-category  

---

### **Scatter Plot - 9**
Used for business analysis to show relationships between variables.  
Point size changes according to a numeric field (e.g., Sales).

- **Scatter Plot (Build)** → Values / X-axis / Y-axis / Legend / Size / Play Axis / Tooltips  
- **Scatter Plot (Format)** → Size and style / Title / X-axis / Y-axis / Legend / Gridlines / Zoom slider / Lines / Markers / Category labels / Plot area background / Trend line / Reference line / Symmetry shading / Ratio line  

**Example 1**  
- **Scatter Plot** →
  - **Values:** Sub-category  
  - **X-axis** → Sales  
  - **Y-axis** → Profit  
  - **Legend** → Category *(Change color)*  
  - **Size** → Quantity *(Bubbles scale with size)*  
  - **Play Axis** → Order Date *(For animation)* 

**Note:**  
To see better visuals, convert **Order Date** to **Date Hierarchy**.  
Use **Ctrl** to select multiple sub-categories.  

---

### **Tree Map - 10**
Visualizes hierarchical data and category-wise contribution using size and color.  
(You can also create sub-trees.)

- **Tree Map (Build)** → Category / Detail / Values / Tooltips  
- **Tree Map (Format)** → Size and style / Title / Legend / Colors / Layout / Data labels / Category labels  

**Example 1 :**  Visualize size-based data diversification.  
- Tree Map → **Category:** Sub-category  
- Tree Map → **Values:** Sales  
- Tree Map → **Detail:** Country *(Remove if too complex)*  

**Example 2**  
- Tree Map → **Category:** Category  
- Tree Map → **Values:** Sales  
- Tree Map → **Detail:** Sub-category  
- Tree Map → **Tooltip:** Profit  

**Calculate Average of Profit in Table**  
- Tooltip → Right-click → Data → Summarization → Average  


