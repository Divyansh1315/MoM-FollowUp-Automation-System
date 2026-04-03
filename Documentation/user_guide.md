# User Guide

## 1. Overview
This system helps track MoM action items and sends automated reminders.

## 2. How to Add a Task
- Open Excel file
- Add new row with:
  - Meeting Name
  - Action Item
  - Responsible Person
  - Responsible Email
  - Target Date
  - Status = Pending

## 3. Status Updates
- Pending → Task is active
- Closed → Stops reminders

## 4. Reminder Behavior
- 2 days before due date
- On due date
- Every 2 days after due date

## 5. Manual Reminder Trigger
- Set "ManualReminderTrigger" = Yes
- System will send reminder immediately

## 6. Important Rules
- Do NOT change column names
- Do NOT delete required fields
- Always update Status after completion

## 7. Error Scenarios
- Missing email → No reminder
- Invalid date → Skipped
- Blank status → Logged as error

## 8. Best Practices
- Update status daily
- Use correct email IDs
- Avoid duplicate rows
