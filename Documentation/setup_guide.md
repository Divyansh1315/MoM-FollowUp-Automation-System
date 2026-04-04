# Setup Guide

## 1. Prerequisites
- Microsoft 365 Account
- Access to SharePoint
- Power Automate access
- Outlook configured

## 2. Clone Repository
git clone <repo-link>

## 3. Excel Setup
- Open Sample_Data.xlsx
- Upload to SharePoint Document Library
- Ensure table name: tbl_MoM_Master

## 4. Power Automate Setup
- Go to Power Automate
- Import Flow (ZIP file from /03_Development/)
- Configure connections:
  - Excel Online
  - Outlook

## 5. Update Configurations
- Update SharePoint file path
- Update table name
- Verify columns mapping

## 6. Run Test
- Trigger flow manually
- Check email delivery
- Validate reminder logic

## 7. Scheduling
- Ensure recurrence trigger is enabled (8 AM IST or as per your convinience)

## 8. Common Issues
- Excel file locked → retry
- Wrong column names → fix schema
