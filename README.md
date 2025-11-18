# Supply Chain Analysis Project

This repository contains the full documentation and structure for the Supply Chain Analysis project, including project planning, stakeholder analysis, database design, and UI/UX design.

---

## 📌 1. Project Planning

The project analyzes supply chain performance using financial, operational, quality, and inventory KPIs.

### Key Planning Components:
- Clear project scope and KPIs
- Defined 4‑week timeline
- Deliverables: analysis, forecasting, dashboard, final report
- Risk assessment and mitigation measures

---

## 📌 2. Stakeholder Analysis

### Stakeholders:
- **Project Team** – Responsible for all analytics and dashboard creation  
- **Instructor** – Reviews and evaluates progress  
- **Management/Decision Makers** – Use insights to improve operations  
- **End Users** – Benefit from optimized supply chain processes  

---

## 📌 3. Database Design

### ERD – Core Entities:
- **Products**: ProductID, ProductType, ManufacturingCost, Price  
- **Suppliers**: SupplierID, SupplierName, Location, LeadTime  
- **Shipments**: ShipmentID, Carrier, Mode, ShippingTime, Cost  
- **Inventory**: StockID, ProductID, StockLevel, Availability, UnitsSold  
- **Quality Inspections**: InspectionID, Result, DefectRate, SupplierID  

### Logical Schema:
Normalized design (up to 3NF) ensuring:
- Reduced redundancy  
- Faster analytical querying  
- Clear relational modeling  

---

## 📌 4. UI/UX Design

### Dashboard Structure:
- Home overview (Financial, Operational, Inventory, Quality)
- Filters for Supplier, Product Type, Location, Carrier
- Visuals: Line charts, bar charts, pie charts, KPI cards
- Drill‑down navigation for detailed insights

### UI Guidelines:
- Consistent color theme  
- Clear typography  
- Simple user navigation  

---

## 📁 Folder Structure (Recommended)

```
📦 SupplyChainProject
│
├── 📂 data
│   ├── cleaned_dataset.csv
│   └── raw_dataset.csv
│
├── 📂 notebooks
│   ├── preprocessing.ipynb
│   ├── analysis_kpis.ipynb
│   └── forecasting.ipynb
│
├── 📂 documentation
│   └── SupplyChain_FullDocumentation.docx
│
├── 📂 dashboard
│   └── powerbi_dashboard.pbix
│
└── README.md
```

---

## 🚀 How to Run the Project

1. Clone the repository:  
   `git clone https://github.com/yourusername/supply-chain-analysis.git`

2. Install required dependencies (Python):  
   `pip install -r requirements.txt`

3. Open Jupyter notebooks for analysis.

4. Open Power BI file to explore the dashboard.

---

## 🧑‍💻 Contributors

- Mohamed  

---

## 📄 License  
MIT License.
