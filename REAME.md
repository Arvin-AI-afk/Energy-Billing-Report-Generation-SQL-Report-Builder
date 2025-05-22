# Energy Billing Report Generation – SQL + Report Builder

## 📘 About this Project

This project provides a semi-automated solution for generating energy billing reports using **SQL Server** and **Report Builder**. It calculates power usage, associated costs, and rack space charges, while supporting both automated meter data and manual inputs.

---

## 🚀 Project Overview

The system aims to replace error-prone manual reporting with SQL-driven automation. Using stored procedures and parameterized templates, it produces structured reports suitable for monthly billing and internal documentation.

🔗 **Project Files**: Custom Report Generation – SQL + Report Builder

---

## 🎯 Project Goals

- Automate the generation of monthly billing reports
- Replicate historical manual report formats using dynamic datasets
- Support manual inputs for offline or missing data
- Accurately calculate power consumption, rack space costs, and total billing
- Enable fast report generation with a user-friendly interface

---

## 🧩 Business Needs

Businesses that monitor energy consumption often need:
- Monthly energy billing based on real-time and offline meter data
- Manual input functionality for incomplete data
- Consistent output matching legacy report formats
- Customizable parameters (client, month, year) for on-demand reporting

---

## 🔧 Key Components

### SQL Server (2022)

- Centralized storage for all meter, client, and billing data
- Stored procedures for:
  - Calculating energy usage (kWh, kVA)
  - Applying offset adjustments for historical alignment
  - Integrating offline meter inputs
  - Generating totals and trends

### Report Builder 3.0

- Uses SQL-stored datasets to:
  - Populate billing tables
  - Create trend visualizations (line/bar charts)
  - Format reports based on selected parameters

---

## 📊 Data Flow Summary

1. **Input Parameters**: Client ID, Month, Year
2. **Stored Procedures**:
   - Retrieve meter and rack data
   - Apply cost formulas and adjustments
3. **Manual Inputs**: Support for offline meters
4. **Report Generation**:
   - Render report via Report Builder using SQL dataset

---

## 💡 Key Insights & Recommendations

- Create a table of offsets or adjustment ratios to align new reports with past values
- Input baseline data to maintain historical consistency
- Minimize user steps for regular monthly reporting (target: 3 clicks)
- Automate data collection or scheduling where possible

---

## 🛠 Tools Used

- **SQL Server 2022**
- **Report Builder 3.0**


---

## 📥 Future Enhancements

- Web-based form for manual input submission
- Email automation or scheduled report runs
- Dashboard view of power/rack trends
- Audit logging and validation checks
