# **Power BI – Cards and Filters**
 
1. Number Card
2. Date Card 
3. Relative Date Filter
4. Text Card
5. Format Card
6. Multi-Row Card
7. Filter on Visual
8. Filter on This Page
9. Filter on All Pages
10. Drill Through


**Note:**  
Drill Through enables users to right-click a data point and navigate to another page to see detailed information related to that selection.


### **1. Number Card**
Used to display a single summary metric (e.g., Total Sales, Profit, or Quantity).

- **Card (Build)** → *Fields*  
- **Card (Format)** → *Size and Style* / *Title* / *Callout Value* / *Category Label*
- **Card Setting**
  - **Card (Format)** → *Size and Style* → *Visual Border* → **Width:** 3px  
  - **Card (Format)** → *Category Label* → **Label:** e.g., *High Sales*  
  - **Card (Format)** → *Callout Value* → **Font Size:** 30 (e.g., *Accessories*)  

Change the name of date fields:  
Right-click on Date field → **Rename for this visual**

Add filter:  
**Filter → Filter on this visual → Add field (e.g., Order Date)**  

---

### **2. Date Card**
Used to show earliest and latest order dates.

**Card 1: Earliest Order Date**
- **Fields** → *Order Date*  
- **Build** → Right-click → *Earliest*  
- **Format** → *Category Label* → On  
- **Format** → *Size and Style → Visual Border* → Width: 3px  

**Card 2: Latest Order Date**
- **Fields** → *Order Date*  
- **Build** → Right-click → *Latest*  
- **Format** → *Category Label* → On  
- **Format** → *Size and Style → Visual Border* → Width: 3px  

**Card 3: Highest Sales**
- **Fields** → *Order Date*  
- **Build** → Add field → *High Sales*  
- **Filter** →
  - Add data field → Order Date
    - Filter type → Top N
    - Show items: 1
    - By value  → Sales  

**Card 4: Highest Discount**
- **Fields** → *Order Date*  
- **Build** → Add field → *High Discount*

**Apply Filter : Highest Discount**
- **Filter** →
  - Add data field → Order Date
    - Filter type → Top N 
    - Show items: 1
    - By value  → Discount
    - Click **Apply Filter**

**Table:** Columns → Order Date, Sales, Discount  

---

### **3. Relative Date Filter**
Used to filter visuals based on a dynamic time range (e.g., last 10 years).

**Card 1: Relative Date**
- **Card (Build)** → Field: *Order Date*  
- **Rename Field:** Right-click → *Rename for this visual → Relative Date*  
- **Format** → *Category Label* → On  
- **Format** → *Visual Border* → Width: 3px  

**Apply Relative Date Filter:**  
- **Filter on this visual → Filter Type:** *Relative Date*  
  - dropdown → *Is in the last* (select)
  - text box→ 10  (wirte)
  - dropdown → *Years*  (select)
  - *Include Today* → ✔️  (check box)
  - Click **Apply Filter**

**Table:** Columns → *Order Date*, *Sales*  
Add same relative date filter on table for matching results.

---

### **4. Text Card**
Used to display top or bottom category names dynamically.

**Card 1: Highest Sales (Sub-Category)**
- **Fields** → *Sub-Category*  
- **Build** → Right-click → *First*  
- **Format** → *Category Label* → On  
- **Format** → *Visual Border* → Width: 3px

**Apply Filter : Highest Sales**
- **Filter** →
  - Add data field → Sub category
    - Filter type → Top N
    - Show items: 1
    - By value  → Discount
    - Click **Apply Filter**

**Card 2: Highest Profit (Sub-Category)**
- Same steps as above, but filter by **Profit**.

**Card 3: Highest Quantity (Sub-Category)**
- Same steps as above, but filter by **Quantity**.

**Table:** Columns → *Sub-Category*, *Sales*, *Profit*, *Quantity*

---

### **5. Format Card**
Used to customize **visual border, background, label size, font size**, and **text appearance** for all cards.

---

### **6. Multi-Row Card**
Displays multiple key values together (e.g., Top 3 Sub-Categories by Sales).

**Multi-Row Card 1: Top 3 Sub-Categories**
- **Fields** → *Sub-Category*, *Sales*, *Profit*, *Discount*  
- **Format** → *Category Label* → On  
- **Format** → *Visual Border* → Width: 3px

**Apply Filter : Highest Sales**
- **Filter** 
  - Add data field → Sub category
    - Filter type → Top N
    - Show items →  3
    - By value  → Sales
    - Click **Apply Filter**

**Supporting Chart:**  
- **Stacked Bar Chart**
  - **Y-Axis:** Category  
  - **X-Axis:** Sales  

---

### **7. Filters on Visual**
Used to filter only one visual.

#### **Pie Chart**
- **Legend:** Category  
- **Values:** Sales 

**Apply Filter : Pie Chart**
- **Filter**
    - Add data field here → Sub category
      - Filter type → Basic filter
      - Search → Select options

#### **Stacked Column Chart**
- **X-Axis:** Sub-Category  
- **Y-Axis:** Sales

**Apply Filter : Stacked Column Chart**  
- **Filter**
    - Add data field here → Sub category
      - Filter type → Basic filter
      - Search → Select options 

#### **Slicer**
- **Field:** Sub-Category  

#### **Table**
- Columns → Sub-Category, Sales  
- Apply same filter on Sub-Category.

**Note:** Slicer filters affect all visuals on the same page.

---

### **8. Filters on Page**
Applies filter to all visuals within the current page.

**Create Pie Chart, Stack Column Chart and Slicer**
- Same steps as above in Filters on Visuals

**Apply Filter on Page**
- **Filter**
  - Filter on this page → Sub-Category
  - Filter Type → Basic Filter 
  - Search → Select options  

- Affects: Pie Chart, Stacked Column Chart, Table, and Slicer.

---

### **9. Filters on All Pages**
Applies filter to every visual across all pages.

**Create Pie Chart, Stack Column Chart table**
- Same steps as above in Filters on Visuals

**Apply Filter on All Page**
- **Filter**
  - Filter on all page → Sub-Category
  - Filter Type → Basic Filter 
  - Search → Select options   

> **Note:** This filter applies to all report pages.

---

### **10. Drill Through**
Used to navigate between pages with specific data context.

**Example Setup**

**Drill Throuh - Sheet**

- **1.1. Stacked Bar Chart**
  - **Y-Axis:** Category  
  - **X-Axis:** Sales
    
- **1.2. Pie Chart**
  - **Legend:** Market  
  - **Values:** Category
     
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


---

