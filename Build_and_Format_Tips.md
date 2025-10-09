# **Power BI Build and Format Tips**

- **Table →  columns :**   best for small, detailed data.
- **Matrix →  rows, columns, values :** best for summarized or large, grouped data (like an Excel Pivot Table).


### **Convert Table into Matrix (and Vice Versa) in Power BI** 

1. **Create a Table** first and add the desired columns (e.g., *Sub-Category*, *Region*, *Sales*).  
2. Once the table is created, **click on the Table visual** and change it to a **Matrix visual** from the visualization pane.  
3. The table will now be converted into a matrix while keeping the same fields.  

**Example:**  
- Create a table and add columns: *Sub-Category*, *Region*, *Sales*.  
- Then click on **Matrix** in the Visualizations pane — the table is now converted into a matrix.

---

### **Copy Tool in Power BI**  
- Right-click on the **square icon** of the visual.  
- Select **Copy → Copy visual**.  
- Then **Paste** it on the same or another report page.  

---

### **Formatting**

| **Section**                 | **Purpose / Description**            | **Key Options**                                                                                                    |
| --------------------------- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Format: Grid**            | Customize table structure and layout | - Set table borders (horizontal & vertical lines) <br> - Adjust border color and thickness <br> - Add cell padding |
| **Format: Values**          | Style data rows for readability      | - Font : increat font size <br> - Change text color <br> - Set background color <br> - Apply alternate row colors                                  |
| **Format: Column Header**   | Customize table headers              | - Set header font style and size <br> - Adjust header background and text color                                    |
| **Format: Totals**          | Format total row                     | - Change total text color and background <br> - Adjust font style and size                                         |
| **Format: Specific Column** | Highlight or style a single column   | - Apply custom color, font, or background to a chosen column                                                       |
---

### **Conditional Formatting (Cell elements)**

Helps **analyze and interpret data visually** by applying color or icons based on values.

**Formatting → Cell elements**

| **Type**             | **Description**                    | **Example**                                                                |
| -------------------- | ---------------------------------- | -------------------------------------------------------------------------- |
| **Background Color** | Shades cells based on value range. | Example: Shade cells by sales value (minimum, center (optional), maximum). |
| **Font Color**       | Changes text color by data value.  | Example: Profit values – low (red), high (green).                          |
| **Data Bars**        | Adds bars to show value magnitude. | Example: Add bars to display discount percentage.                          |
| **Icons**            | Uses icons to indicate trends.     | Example: Show up/down arrows for profit.                                   |


---

| **Type**             | **Usage / Description**                                                     | **Example**                                                                |
| -------------------- | --------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| **Background Color** | Apply color shading to cells based on value ranges to highlight variations. | Example: Shade cells by sales value (minimum, center (optional), maximum). |
| **Font Color**       | Change text color dynamically based on data values for better readability.  | Example: Profit values – low (red), high (green).                          |
| **Data Bars**        | Display horizontal bars within cells to visually represent data magnitude.  | Example: Show bars to illustrate discount percentages.                     |
| **Icons**            | Add symbols or icons to convey trends or status at a glance.                | Example: Display up/down arrows for profit trends.                         |


---

| **Type**             | **Usage / Description**                   | **Example**                                                    |
| -------------------- | ----------------------------------------- | -------------------------------------------------------------- |
| **Background Color** | Color cells based on value ranges         | Example: Shade cells by sales value (low = light, high = dark) |
| **Font Color**       | Change text color according to data value | Example: Profit values – low (red), high (green)               |
| **Data Bars**        | Display bar visual within a cell          | Example: Add bars to show discount percentage visually         |
| **Icons**            | Add icons for quick insights              | Example: Display up/down arrows for profit trends              |

---

### **Change Aggregation**

| **Table**          | **Steps**                                                                     | **Description**                              |
| ------------------ | ----------------------------------------------------------------------------- | -------------------------------------------- |
| **Average Profit** | Import **Profit** → Right-click on field → Select **Average**                 | Shows mean profit per record                 |
| **Count Profit**   | Import **Profit** → Right-click → Select **Count**                            | Displays number of profit records            |
| **% Profit**       | Import **Profit** → Right-click → **Show Values As → Percent of Grand Total** | Shows profit as a percentage of total profit |

---

### **Hierarchies in Power BI**  

**Hierarchies** help organize data into multiple levels within visuals (such as Matrix or Charts), enabling drill-down or expansion from summary to detailed views.  

**Steps:**  
1. Select the **Matrix** visual.  
2. Add fields to define a hierarchy structure.  

**Example:**  
- **Rows →** Category → Region → Segment  
- **Columns →** Order Date (Year → Quarter → Month → Day)  
- **Values →** Sales  

This configuration allows analysis of sales data across different time periods and categories, providing the ability to drill down for detailed insights.

---
