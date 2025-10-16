## Functions and Advance Charts




---

#### **Power BI – Bookmark**

Bookmarks in Power BI are used to capture the current state of a report page (including filters, visuals, and visibility) so users can switch between customized views with a single click.

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

### **Drill Through Action**

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
