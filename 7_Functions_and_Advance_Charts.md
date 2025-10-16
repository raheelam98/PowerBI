## Functions and Advance Charts

1. Basic - Insert Image / Text / Shapes /  Buttons  and Web URL Action
2. Button and Navigation 
3. Bookmark Action
4. Drill Through Action
5. KPI Visualization Tool
6. Key Influencers
7. Decomposition Tree
8. Python & R Scripting  (do later)
9. Third-Party Extension Icon (do later)

---

#### **3- Power BI – Bookmark**

**Purpose:**  
Bookmarks are used to **capture a specific view or state of a report page** (including filters, visuals, and visibility) so users can switch between customized views with a single click.

#### **Pie Chart**
- **Legend:** Category  
- **Values:** Sales  

#### **Stacked Column Chart**
- **X-Axis:** Market  
- **Y-Axis:** Category  

#### **Create Buttons**
- **Button 1:** Show Sales  
- **Button 2:** Show Market  
- **Button 3:** Show All  

**Steps to Create Bookmarks**

**Step 1: Enable Bookmark & Selection Pane**
- Go to **View → Bookmarks  → Selection**  
- Make sure both are turned **On**


**Step 2: Create “Show Sales” Bookmark**
1. In the **Selection Pane**, hide → *Category by Market* visual.  
2. In the **Bookmarks Pane**, click **Add** → Rename it → **Show Sales**.  
3. Select **Show Sales Button** →  
   - **Format → Action**  
     - **Action → Type:** Bookmark  
     - **Bookmark → Show Sales**

**Step 3: Create “Show Market” Bookmark**
1. In the **Selection Pane**, hide → *Category by Sales* visual.  
2. In the **Bookmarks Pane**, click **Add** → Rename it → **Show Market**.  
3. Select **Show Market Button** →  
   - **Format → Action**  
     - **Action → Type:** Bookmark  
     - **Bookmark → Show Market**


#### **Step 4: Create “Show All” Bookmark**
1. Make both visuals **visible** in the Selection Pane.  
2. In the **Bookmarks Pane**, click **Add** → Rename it → **Show All**.  
3. Select **Show All Button** →  
   - **Format → Action**  
     - **Action → Type:** Bookmark  
     - **Bookmark → Show All**


**Tip:**  
Bookmarks can also be combined with buttons, slicers, and filters to create interactive report navigation or storytelling experiences in Power BI.

---

### **4- Drill Through Action**

**Purpose:**  
Allows users to **navigate to another report page** that shows **detailed information** about a selected data point.

- **1.1. Stacked Bar Chart**
  - **Y-Axis:** Category  
  - **X-Axis:** Sales
    
- **1.2. Pie Chart**
  - **Legend:** Market  
  - **Values:** Category

- **1.3. Create Buttons**
   - **Button 1:** Sales Detail  
   - **Button 2:** Market Detail
     
- **2. Sheet 1 : Tables**
  - Table 1 → Sub-Category, Sales  
  - Table 2 → Order Date, Sales  
  - Table 3 → Category, Sales
 
- **3. Sheet 2 : Tables**
  - Table 1 → Customer Name, State  
  - Table 2 → Market, Sales
  
**Apply Drill Through on Sheet 1**
- **Format**
  - **Page Information**
    - **Name:** Drill Sheet One  (Sheet Name)
    - **Page Type:** Drillthrough  
    - **Keep All Filters / Cross-Report:** Off  
    - **Drill Through From:** Category  

**Apply Drill Through on Sheet 2**
- **Format**
  - **Page Information**
    - **Name:** Drill Sheet Two  (Sheet Name)
    - **Page Type:** Drillthrough  
    - **Keep All Filters / Cross-Report:** Off  
    - **Drill Through From:** Market

**Apply Drill Through on Button 1 (Sales Detail)**
- **Format Button**
  - **Action**
    - **Type:** Drillthrough   
    - **Destination:** Sheet Name (Sheet 1)

**Apply Drill Through on Button 2 (Market Detail)**
- **Format Button**
  - **Action**
    - **Type:** Drillthrough   
    - **Destination:** Sheet Name (Sheet 2)

---

### **5- KPI Visualization Tools**

**Purpose:**  
Used to measure **Key Performance Indicators (KPIs)** — shows how actual performance compares against a defined target over time.

- KPI (Build) —> Value / Trend axis / Target  (target is important)
- KPI (Format) —> size and style / title / callout value / icons / trend axis / target label / date


#### **KPI - Build Pane**
- **Value:** Discount  
- **Trend Axis:** Order Date  
  - Use *Date Hierarchy* → Expand all except *Year*  
- **Target:** Order Date *(Target field is important)*


#### **Supporting Visuals**

**Table**
- **Columns:** Order Date  
  - Use *Date Hierarchy* → Expand all except *Year* and *Quarter*  

**Slicer**
- **Field:** Order Date (Date Hierarchy)  
  - **Format:** Vertical List  

---

### **6- Key Influencers**

**Purpose:**  
Identifies and explains factors that influence a key metric.

- Key Influencers  (Build) —> analyze / explain by / expand by  (take multiple values in explain by )
- KPI (Format) —> size and style / title / callout value / icons / trend axis / target label / date


#### **Build Pane**
- **Analyze:** Sales  
- **Explain By:** Sub Category, Product Name *(Can take multiple values)*

---

### **7- Decomposition Tree**

**Purpose:**  
Used to break down a measure (like sales or profit) across multiple dimensions to analyze root causes.

- Decomposition Tree  (Build) —> analyze / explain by / expand by  (take multiple values in explain by )

#### **Build Pane**
- **Analyze:** Category  
- **Explain By:** Sub Category, Quantity, Profit, Sales  

---

