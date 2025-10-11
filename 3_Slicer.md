# Power BI - Slicer  

**Slicer :** A slicer is a visual filter that allows users to segment and analyze data interactively.

- Slicers enhance user experience by enabling dynamic filtering
- Combine slicers with visuals (tables, charts) for interactive reports
- Customize slicer appearance to match report design


### **Slicers – Topics**
1. **Create Slicers**  
2. **Text Slicer**  
3. **Format Text Slicer**  
4. **Date Slicer**  
5. **Format Date Slicer**  
6. **Number Slicer**

---

### Power BI Slicer 

A **Slicer** in Power BI acts as a dynamic filter that allows users to interactively control visuals such as tables, charts, and KPIs.

- **Build → Slicer → Field**
- **Format → Size & Style / Title / Slicer Settings / Slicer Header / Values / Hierarchy**

---

### Power BI Slicer Customization: Shape, Header, and Value Formatting

---

### **Slicer Settings** : **Adjust slicer layout**  
- **Format → Slicer Settings → Option**  
  - **Style** → Vertical list / Title / Between / Before / After / Dropdown / Relative date / Relative time  

**Selection Options**  
- **Format → Slicer Settings → Selection**
  - Single Select  
  - Multi-Select with CTRL  
  - Select All
  
**Reset Slicer**  
- **Format → Slicer Settings → Reset to Default**

---

### **Slicer Header** : **Customize header**  
- **Format → Slicer Header → Text**  
  - Title Text / Font / Font Color  
- **Format → Slicer Header → Border**  
  - Position / Color / Line Width  
- **Format → Slicer Header → Background**  
  - Color  
- **Format → Slicer Header → Pending Icon**  
  - Color / Transparency  

---

### **Slicer Value** : **Format slicer values**  
- **Format → Value → Values**  
  - Font / Font Color / Padding  
- **Format → Value → Border**  
  - Border Position / Color / Line Width  
- **Format → Value → Background**  
  - Color  
- **Format → Value → Reset to Default**

---

### **Slicer – Date** : **Date / Hierarchy Setup**  
- **Slicer → Field → (Drag and Drop Date Column)**  
- **Right-click on Date Column → Data →**  
  - Date → Date Column / Date Hierarchy  

---

### Visual Filtering in Power BI: Using Slicers for Data Interaction

---

### 🎯 Basic Slicer Setup

**Steps**
1. Click **Slicer**.
2. Go to **Field** → Drag and drop **Category**.
3. Create a **Horizontal Slicer**.

**Path:**  
`Format → Slicer Settings → Option (Title)`

---

### 📝 Text Slicer

**Steps**
1. Click **Slicer** → Drag and drop **Category** into **Field**.  
2. In **Table**, drag and drop **Sub-Category** and **Sales** into **Columns**.  
3. Selecting a category in the slicer filters the table accordingly.  
4. To select multiple categories → Hold **Ctrl + Click**.

---

### 🪜 Slicer with Hierarchy

**Steps**
1. Slicer → Field → Drag and drop **Category** and **Sub-Category**.  
2. Slicer → Field → Drag and drop **Segment**.  
3. Slicer → Field → Drag and drop **Region**.

---

### 🥧 Slicer + Pie Chart

**Steps**
1. **Pie Chart → Legend:** Drag and drop **Category**.  
2. **Pie Chart → Value:** Drag and drop **Sub-Category**.

---

### ✏️ Format Text Slicer

**Steps**
1. **Table → Columns:** Sub-Category, Sales.  
2. **Pie Chart → Legend:** Category, Sub-Category.

---

### 🔘 Multi-Select Without CTRL

**Steps**
1. **Slicer → Field:** Category.  
2. **Format → Slicer Settings → Selection:** Turn **Off Multi-Select with CTRL**.

---

### 🙈 Hide Field Name from Slicer

**Path:**  
`Format → Slicer Header → Off`

---

### 🧭 Slicer as Dashboard

Create a **Horizontal Slicer** that functions like a dashboard.

**Path:**  
`Format → Slicer Settings → Option (Title)`

---

### 🏙️ Slicer as Buttons – Format City

**Steps**
1. **Slicer → Field:** City.  
2. **Format → Slicer Settings → Option (Title)**.  
3. **Format → Value:** Adjust **Font Size** and **Background Color**.

---

### 📅 Date Slicer (Between Style)

**Steps**
1. **Table → Columns:** Order Date, Profit.  
2. **Slicer → Field:** Order Date.  
3. **Format → Slicer Settings → Option:** Style → **Between**.

---

### ⏰ Relative Time Date Slicer

**Steps**
1. **Slicer → Field:** Order Date.  
2. **Format → Slicer Settings → Option:** Style → **Relative Time**.

---

### 🗓️ Date Hierarchy Slicer (Dropdown Style)

**Steps**
1. **Table → Columns:** Order Date, Profit.  
2. **Slicer → Field:** Order Date.  
3. **Right Click → Data → Date Hierarchy.**  
4. **Format → Slicer Settings → Option:** Style → **Dropdown**.

---

### 📈 Date Hierarchy Slicer (Vertical Line Style)

**Steps**
1. **Slicer → Field:** Order Date.  
2. **Right Click → Data → Date Hierarchy.**  
3. **Format → Slicer Settings → Option:** Style → **Vertical Line**.

---

### 🧭 Date Buttons (Title Style)

**Steps**
1. **Slicer → Field:** Order Date.  
2. **Format → Slicer Settings → Option:** Style → **Title**.  
3. **Format → Slicer Header:** Off.  
4. **Format → Value:**  
   - Font Color → White  
   - Background → Blue  

---

### 🎨 Date Hierarchy Dropdown with Formatting

**Steps**
1. **Slicer → Field:** Order Date.  
2. **Right Click → Data → Date Hierarchy.**  
3. **Format → Slicer Settings → Option:** Style → **Dropdown**.  
4. **Format → Value:**  
   - Font Color → Red  
   - Background → Grey  

---

### 🍩 Donut Chart with Slicer

**Steps**
1. **Legend →** Order Date.  
2. **Value →** Sum.  

---

### 🔢 Number Slicer

**Steps**
1. **Table → Columns:** Customer Name, Sales.  
2. **Slicer → Field:** Quantity.  
3. **Slicer → Field:** Sales.  




