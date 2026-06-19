# payroll_reconciliation
This tool is actively used in a real payroll environment and has delivered measurable improvements:  Faster reconciliation  Reduced manual errors  Accurate departmental salary allocation  Clear audit trail for payroll adjustments  Improved confidence in monthly and year‑end reporting
Payroll Reconciliation & Tax Apportioning Automation (Python, Jupyter)
A production‑used payroll reconciliation tool built in Python (Jupyter) to automate and validate complex payroll datasets used in a UK education‑sector finance environment.
The payroll system currently exports ~99 columns, including multiple deduction types, contributions, and role‑based pay elements. This project streamlines the data, groups deductions by category, and performs automated checks to ensure payroll accuracy across departments.

Key Features
1. Automated Grouping of Payroll Deductions
The script consolidates and groups payroll deductions into meaningful categories (e.g., Tax, NI, Pension, Student Loans, OMP, SSP).
This reduces manual work and ensures consistent reporting across months and payroll cycles.

2. Intelligent Tax Apportioning for Multi‑Role Staff
In the payroll system, tax is allocated entirely to the first role, even when a staff member holds two positions.
This leads to incorrect departmental salary reporting.

The code automatically:
Detects staff with multiple roles
Calculates proportional tax distribution based on gross pay
Reallocates tax across roles
Ensures departmental salary costs are reported accurately

This logic is essential for correct budget monitoring, departmental reporting, and year‑end reconciliation.

3. Mismatch Detection & Exception Reporting
Payroll data is not always perfect. Sometimes:

A staff member appears in one dataset but not another
Role codes don’t match
Deductions don’t align with expected totals
The script identifies:
Missing matches
Inconsistent records
Staff requiring manual payslip checks

These exceptions are flagged clearly so the finance team can review payslips and make necessary adjustments before final reporting.

4. Clean, Reproducible Workflow
The notebook provides:
Clear data‑loading steps
Transformation logic
Validation checks
Summary outputs for finance reporting

It is designed to be readable, auditable, and easy to maintain.
