# 📌 MoM Follow-Up Automation System

> **Automating accountability. Enforcing governance. Designing for scale.**

---

## 🚀 Project Overview

The **MoM (Minutes of Meeting) Follow-Up Automation System** is an enterprise-style automation solution built using Microsoft 365 tools to streamline tracking and execution of meeting action items.

This project addresses a common organizational gap — **manual follow-ups leading to missed deadlines, poor visibility, and lack of accountability**.

The system automates reminders, enforces validation, maintains auditability, and is designed with a **future-ready architecture for enterprise scalability**.

---

## 🎯 Business Problem

In most organizations, MoM tracking is handled manually via Excel:

- ❌ Action items get missed  
- ❌ No proactive reminders  
- ❌ Manual tracking is time-consuming  
- ❌ No audit trail  
- ❌ Accountability is unclear  

---

## ✅ Solution

This project introduces a **Power Automate-based reminder engine** integrated with Excel (SharePoint) and Outlook to:

- 🔔 Send automated reminders before and after due dates  
- 📊 Track action items centrally  
- 📩 Notify responsible owners automatically  
- 🧾 Maintain audit logs  
- ⚠️ Handle data validation errors  
- 🔄 Enable manual reminder triggers  

---

## 🏗️ Architecture Overview

### 🔹 Data Layer
- Excel Online (stored in SharePoint)
- Structured table for MoM tracking

### 🔹 Automation Layer
- Power Automate Cloud Flow
- Recurrence-based trigger

### 🔹 Communication Layer
- Outlook Email Service

---

## ⚙️ Key Features

### 📅 Smart Reminder Engine
- 3 days before due date  
- On due date  
- Every 2 days after due date (until completion)

### 🧠 Intelligent Logic
- Sends reminders only for **pending tasks**
- Stops automatically when status = **Closed**
- Prevents duplicate reminders

### 🔁 Manual Trigger Support
- Allows PMO to send reminders on-demand

### 🧾 Audit & Tracking
- Reminder counter  
- Last reminder tracking  
- Audit log support  

### ⚠️ Data Validation Layer

Handles:

- Missing target dates  
- Missing emails  
- Invalid date formats  
- Blank status  

---

## 📊 Data Model (Excel Schema)

| Column | Description |
|------|-------------|
| TaskID | Unique identifier |
| MeetingName | Meeting reference |
| MeetingDate | Date of meeting |
| ActionItem | Task description |
| ResponsiblePerson | Owner |
| ResponsibleEmail | Email for reminders |
| TargetDate | Due date |
| Status | Task status |
| Remarks | Additional notes |
| ReminderCounter | Tracks reminders sent |
| LastReminderSent | Timestamp |
| ManualReminderTrigger | On-demand trigger |
| ReminderEligible | Logic flag |
| ErrorFlag | Validation tracking |
| ErrorMessage | Error details |
| ManagerEmail | Future escalation |
| EscalationFlag | Phase 2 |

---

## 🔄 Automation Flow Logic

```text
Recurrence Trigger (Daily / Configurable)
        ↓
Read Excel Table
        ↓
Data Validation Layer
        ↓
Check Reminder Eligibility
        ↓
Apply Reminder Rules
        ↓
Send Email via Outlook
        ↓
Update Reminder Counter & Logs
```

---

## 🛡️ Error Handling Strategy

| Risk | Mitigation |
|------|------------|
| Invalid data | Validation layer |
| Missing fields | PMO notification |
| Flow failure | Logging + retry |
| Excel locking | Retry policy |
| Duplicate emails | Reminder flag logic |

---

## 📈 Scalability & Design Thinking

This solution is intentionally designed as **Phase-Based Architecture**:

### Phase 1 (Current)
- Excel-based tracking  
- Automated reminders  
- Validation layer  

### Phase 2 (Planned)
- Manager escalation  
- Power BI dashboard  
- Audit logging system  

### Phase 3 (Enterprise Scale)
- Migration to Dataverse  
- Power Apps UI  
- Row-level security  
- Advanced analytics  

---

## 🧠 Architectural Principles Applied

- ✔ Start Lean, Design for Scale  
- ✔ Separation of Data, Logic, Communication  
- ✔ Cost-efficient (No premium licensing)  
- ✔ Migration-ready design (Excel → Dataverse)  
- ✔ Governance-first thinking  

---

## 🎯 Success Metrics

- ✅ No task crosses due date without reminder  
- ✅ Reduced manual follow-up effort  
- ✅ Improved accountability  
- ✅ Visibility into pending tasks  
- ✅ Structured tracking system  

---

## 🛠️ Tech Stack

- Microsoft Power Automate  
- Microsoft Excel (Online)  
- Microsoft SharePoint  
- Microsoft Outlook  

---

## 📌 Key Learnings & Skills Demonstrated

### 👨‍💻 Technical Skills
- Power Automate workflow design  
- Data validation and error handling  
- Automation logic design  
- Excel schema structuring  

### 🧠 Architectural Thinking
- Scalable system design  
- Phase-based roadmap planning  
- Migration strategy (Dataverse readiness)  
- Performance & limitation awareness  

### 📋 Project Management Skills
- Requirement gathering  
- BRD & SDD documentation  
- Stakeholder thinking (PMO perspective)  
- Risk identification  
- Governance planning  

---

## 💡 Portfolio Value

This project demonstrates:

> “Not just building automation, but designing a scalable, governance-driven system aligned with enterprise practices.”

---

## 🔮 Future Enhancements

- Power BI dashboards  
- SLA tracking  
- Department-level reporting  
- Dataverse migration  
