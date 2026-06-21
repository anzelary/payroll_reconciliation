# Payroll Reconciliation & Tax Apportioning Automation (Python, Jupyter)

> **Data Privacy Notice:**  
> This project is used in an actual payroll reconciliation workflow; however, the version published in this repository contains **only fully fictional sample data**.  
> No real employee information, identifiers, payroll values, or confidential system details are included.  
> Column names reflect typical fields found in standard payroll exports and do not contain any sensitive or proprietary information.


This tool is actively used in a real payroll environment and has delivered measurable improvements:  Faster reconciliation,  Reduced manual errors,  Accurate departmental salary allocation,  Clear audit trail for payroll adjustments,  Improved confidence and consistency in monthly and year‑end reporting.

## Overview

Payroll exports often allocate all Tax and NIC to the first role and split pay elements across multiple similarly‑named columns (e.g., *Overtime 1.0*, *Overtime 1.3*, *Overtime 2.0*).  
This script standardises the dataset, redistributes deductions proportionally, and validates totals against the original report.

The output includes a detailed cleaned dataset and a department‑level summary suitable for finance, audit, and budget monitoring.

---



## Key Features
-**`1. Automated Grouping of Related Columns`** <br>
Consolidates fragmented pay types (e.g., “Overtime 1.0”, “Overtime 1.3”, “Overtime 2.0”  into unified categories such as **Overtime**), reducing noise and improving reporting clarity.

-**`2. Tax/NIC Apportioning for Multi‑Role Staff`** <br>
Redistributes deductions proportionally based on each role’s gross pay, correcting the common issue where the payroll export assigns all Tax/NIC to the first role.In the payroll system.  The code automatically, 
detects staff with multiple roles and calculates proportional tax distribution based on gross pay. Ensures departmental salary costs are reported accurately. This logic is essential for correct budget monitoring, departmental reporting, and year‑end reconciliation.

-**`3. Mismatch Detection & Exception Reporting`** <br>
Payroll data is not always perfect. Sometimes, a staff member appears in one dataset but not another, deductions don’t align with expected totals, etc. The script identifies missing matches. These exceptions are flagged clearly so the finance team can review payslips and make necessary adjustments before final reporting.

-**`4. Export the simplified detailed reeport to Excel`** <br>
Includes grouped columns, apportioned deductions, and cleaned numeric fields.

-**`5. Export the Summary by Department report to Excel`** <br>
Aggregates gross pay, employer costs, and apportioned deductions by department for finance and budget monitoring.

-**`6. Clean, Reproducible Workflow`** <br>
The notebook provides clear data‑loading steps, transformation logic, alidation checks and summary outputs for finance reporting


## Technologies Used

- **Python** (pandas, numpy, openpyxl, os)
- **Excel** for final reporting
- **Jupyter Notebook / VS Code** for development and testing

---
## Files Included
- `fullpaymentdetails.csv` – fake payroll data created for demonstration only
- `payrollReconciliation.ipynb` – main Python file
- `examples.jpg` – illustration of the main features of the precessed reports
  
---
## Skills Demonstrated
- Loading and processing datasets using `pandas` and `os`
- Data Cleaning & Pre=processing
- Implementing logic for filtering and grouping data
- Implementing logic for apportioning data
- Problem solving & Debugging
- Reconciliation & Validation
- Automated Excel export using `openpyxl` and `pd.ExcelWriter`
- Automation of Financial Workflows
- Business Logic Implementation (TAX/NIC apportion)
- Documentation & Reporting

---
## Contact

Created by **Anzela Rizakova**  
For collaboration or questions, feel free to reach out via GitHub.
