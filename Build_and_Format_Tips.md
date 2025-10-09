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

**Format → Cell elements**

| **Type**             | **Description**                    | **Example**                                                                |
| -------------------- | ---------------------------------- | -------------------------------------------------------------------------- |
| **Background Color** | Shades cells based on value range. | Example: Shade cells by sales value (minimum, center (optional), maximum). |
| **Font Color**       | Changes text color by data value.  | Example: Profit values – low (red), high (green).                          |
| **Data Bars**        | Adds bars to show value magnitude. | Example: Add bars to display discount percentage.                          |
| **Icons**            | Uses icons to indicate trends.     | Example: Show up/down arrows for profit.                                   |

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

### **Power BI Drill Options Toolbar**

| Icon                      | Option                                                                                                 | 
| ------------------------- | ------------------------------------------------------------------------------------------------------ | 
| 🔽 **Drill on Rows**      | Specify whether you want to drill through rows or columns in a visual (mainly used in matrix visuals). |             
| ⭡ **Up Arrow**            | Move up one level in the data hierarchy.                                                               |             
| ⭣ **Down Arrow**          | Drill down into the next level of the hierarchy for a selected data point.                             |             
| ⭣⭣ **Double Down Arrows** | Drill down all at once across all categories.                                                          |             
| ⭳ **Split Arrows**        | Expand all levels of the hierarchy to view multiple levels together.                                   |             
| ⛃ **Filter Icon**         | Apply filters directly on the visual for focused analysis.                                             |             
| ⤢ **Focus Mode Icon**     | Expand the visual to full screen for detailed exploration.                                             |            
| ⋯ **More Options**        | Access additional settings such as sorting, exporting data, or formatting visuals.                     |             

**Purpose**

The Drill Options Toolbar empowers users to:

- 🔍 Navigate between different levels of data hierarchies.
- 📊 Drill down for detailed insights or roll up for summarized views.
- 🎛️ Apply filters and focus on specific visual elements.

---

### **Grand Total and Subtotal in Matrix Visualization**

- **Subtotals** summarize data for each row or column group.
- **Grand totals** display the overall summary across all categories.

**Step 1: Add Data to Matrix**
- **Rows** → Add **Category** and **Sub-Category**  
- **Values** → Add **Sales**

**Step 2: Configure Row Subtotals**
1. Go to **Format** → **Row subtotal** → **On**
2. **Row subtotal options:**
   - **Row level** → All / Category
   - **Value** → Set **Text color** or **Background color**  
     - Example: **Blue color** on total rows

**Step 3: Configure Row Grand Total**
1. Go to **Format** → **Row grand total**
2. Apply **Background color** → **Brown** (for grand total rows)

**Step 4: Configure Column Subtotals**
1. Add **Market** to **Columns**
2. Go to **Format** → **Column subtotal** → **On**
3. **Values** → Apply **Background color**  
   - Example: **Pink color** on column totals

**Summary**
- **Row Subtotals:** Enabled with blue highlights  
- **Row Grand Total:** Highlighted in brown  
- **Column Subtotals:** Enabled with pink highlights


This setup makes **Power BI Matrix reports** visually clear by distinguishing subtotals and grand totals with colors.

