# Power BI Slicer Guide

**Slicer :** A slicer is a visual filter that allows users to segment and analyze data interactively.

- Slicers enhance user experience by enabling dynamic filtering
- Combine slicers with visuals (tables, charts) for interactive reports
- Customize slicer appearance to match report design

**How to add a slicer:**
- Go to `Insert` → `Slicer`
- Drag and drop the desired field (e.g., Category)

### 🔧 Slicer Layouts & Types

1. **Horizontal Slicer**
- Format → Slicer settings → Orientation → `Horizontal`
- Useful for dashboard-style button layouts

2. **Text Slicer**
- Drag a text field (e.g., Category) into the slicer

3. **Hierarchical Slicer**
- Drag multiple fields into the slicer (e.g., Sub-category, Segment)

4. **Button-style Slicer (City)**
- Drag `City` field into slicer
- Format → Slicer settings → Options → Enable `Title`
- Format → Values → Customize font size and background color

---

### 🎛️ Slicer Formatting Options

**✅ Multi-select Without CTRL**
- Format → Selection controls → Turn off `Multi-select with CTRL`

**🚫 Hide Field Name**
- Format → Slicer header → Toggle `Off`

---

## 📊 Slicer Interactions with Visuals

**Table Filtering**
- Add a table with fields like `Sub-category`, `Sales`
- Selecting a slicer value filters the table
- Hold `Ctrl` to select multiple categories (or enable multi-select)

**Pie Chart Filtering**
- Pie chart setup:
  - Legend → Drag `Category`
  - Values → Drag `Sub-category`
- Slicer selections dynamically filter the chart

## 🆕 Creating New Slicers
- Add multiple slicers for enhanced dashboard interactivity
- Use horizontal layout for button-style slicers


