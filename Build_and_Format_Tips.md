# **Power BI Build and Format Tips**

## **Table : columns** 

#### **Table Formatting**


| **Section**                 | **Purpose / Description**            | **Key Options**                                                                                                    |
| --------------------------- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Format: Grid**            | Customize table structure and layout | - Set table borders (horizontal & vertical lines) <br> - Adjust border color and thickness <br> - Add cell padding |
| **Format: Values**          | Style data rows for readability      | - Font : increat font size <br> - Change text color <br> - Set background color <br> - Apply alternate row colors                                  |
| **Format: Column Header**   | Customize table headers              | - Set header font style and size <br> - Adjust header background and text color                                    |
| **Format: Totals**          | Format total row                     | - Change total text color and background <br> - Adjust font style and size                                         |
| **Format: Specific Column** | Highlight or style a single column   | - Apply custom color, font, or background to a chosen column                                                       |

#### **Table Conditional Formatting : Cell elements**

Helps **analyze and interpret data visually** by applying color or icons based on values.

**Formatting → Cell elements**

| **Type**             | **Usage / Description**                   | **Example**                                                    |
| -------------------- | ----------------------------------------- | -------------------------------------------------------------- |
| **Background Color** | Color cells based on value ranges         | Example: Shade cells by sales value (low = light, high = dark) |
| **Font Color**       | Change text color according to data value | Example: Profit values – low (red), high (green)               |
| **Data Bars**        | Display bar visual within a cell          | Example: Add bars to show discount percentage visually         |
| **Icons**            | Add icons for quick insights              | Example: Display up/down arrows for profit trends              |

#### **Change Aggregation**

| **Table**          | **Steps**                                                                     | **Description**                              |
| ------------------ | ----------------------------------------------------------------------------- | -------------------------------------------- |
| **Average Profit** | Import **Profit** → Right-click on field → Select **Average**                 | Shows mean profit per record                 |
| **Count Profit**   | Import **Profit** → Right-click → Select **Count**                            | Displays number of profit records            |
| **% Profit**       | Import **Profit** → Right-click → **Show Values As → Percent of Grand Total** | Shows profit as a percentage of total profit |

---

## **Matrix : rows, columns, values**
