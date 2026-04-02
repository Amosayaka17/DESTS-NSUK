# Digital Exam Script Tracking System (DESTS)
## Integrated Design Project
**Nasarawa State University, Keffi (NSUK)**
**Department:** Cybersecurity
**Focus Area:** Education Sector

---

## What is the problem of your target user?

Students at Nasarawa State University Keffi (NSUK) frequently submit examination scripts only to be told their script is missing during result processing, leaving them with no grade, no evidence, and no recourse — despite having sat and submitted the examination. This leads to unjust academic outcomes, repeated courses, delayed graduation, and a complete loss of trust in the examination process.

---

## The 5 Whys Analysis

**[W1] Why does this problem occur?**
Because there is no digital tracking system to record, monitor, or confirm the movement of individual examination scripts from the moment a student submits them to the point where results are entered.

**[W2] Why does W1 occur?**
Because the entire examination script workflow — collection, storage, transfer, and marking — is handled manually and physically, with no count verification or individual identification at any stage of the process.

**[W3] Why does W2 occur?**
Because script collection, departmental storage, and handoff to lecturers are managed separately by different individuals using paper-based methods, with no unified system connecting these stages or flagging discrepancies between them.

**[W4] Why does W3 occur?**
Because there has been no institutional investment or technical effort directed at digitizing the examination script management process, despite the critical role it plays in determining students' academic outcomes.

**[W5] Why does W4 occur? (Root Cause)**
Because university administrations traditionally treat examination script management as a purely physical, administrative task — failing to recognize that the absence of a digital accountability trail creates a system where scripts can disappear without detection, and where the burden of proof falls entirely on the student rather than the institution.

---

## Your Objective and Potential New Idea That Benefits the User

**Objective:**
To eliminate the vulnerability of the physical examination script process by introducing full digital accountability at every stage — from the moment a student submits their script to the moment their result is uploaded — making it impossible for a script to go missing without an immediate, traceable alert.

**New Idea:**
Develop a secure, web-based **Digital Exam Script Tracking System (DESTS)**. This platform would assign every examination script a unique digital identity at the point of submission. It would track the script in real-time through each stage of the process — collection, storage, lecturer handoff, marking, and result entry. Each stage would require digital confirmation from the responsible staff member, and any count mismatch would trigger an automatic alert to the department. Students would be able to check the live status of their own script at any time using their matric number, giving them full visibility and a digital record as evidence in the event of a dispute.

---

## System Design

### The Three Danger Zones in the Current Process

| Zone | Stage | The Problem |
|------|-------|-------------|
| 🔴 Zone 1 | Script Collection | Scripts collected as a bulk pile with no individual tracking |
| 🔴 Zone 2 | Physical Storage | Scripts stored physically with no monitoring or oversight |
| 🔴 Zone 3 | Handoff to Lecturer | No count verification — missing scripts go unnoticed until results time |

### How DESTS Fixes Each Zone

```
ZONE 1 FIX — Script Collection
Every script is logged individually at submission.
System records: Matric No., Course, Hall, Time, Invigilator.
Alert raised immediately if final count does not match registered students.

ZONE 2 FIX — Physical Storage
Department officer digitally confirms receipt of the script bundle.
System records storage location and responsible officer.
Any gap between collected and received count triggers an alert.

ZONE 3 FIX — Handoff to Lecturer
Lecturer digitally confirms how many scripts were received.
System identifies exactly which script(s) are unaccounted for.
No result can be uploaded for a script that was never logged.
```

### The Four Portals

| Portal | User | Function |
|--------|------|----------|
| 🔐 Login Page | All users | Role-based authentication |
| 👮 Invigilator Portal | Invigilators | Log every script at collection, view running count |
| 👨‍🏫 Lecturer Portal | Lecturers | Confirm receipt, flag missing scripts, upload results |
| 👨‍🎓 Student Portal | Students | Check real-time script status using matric number |

---

## Cybersecurity Features

| Feature | Description | Principle Applied |
|---------|-------------|------------------|
| **Authentication** | All staff log in with verified credentials before accessing the system | Identity verification |
| **Role-Based Access Control** | Each user can only access features relevant to their role | Principle of Least Privilege |
| **Audit Trail** | Every action is permanently logged with a timestamp and the responsible user | Full accountability |
| **Tamper Detection** | System raises an alert if any record is edited or deleted outside of normal workflow | Data integrity |
| **Data Encryption** | All student records are stored in encrypted form in the database | Data confidentiality |
| **Unique Script ID** | Every answer booklet is assigned a unique identifier at the point of logging | Non-repudiation |

---

## Expected Impact

| Situation | Before DESTS | After DESTS |
|-----------|-------------|------------|
| Script goes missing | Nobody knows where or when | System shows exact last logged location and handler |
| Accountability | Zero — blame is passed around with no proof | Every handler is identified with a timestamp |
| Student appeal | No evidence to support the student's case | Full digital audit trail serves as proof |
| Department oversight | Blind until results time | Real-time dashboard with live script counts |
| Result tampering | Possible without detection | Audit trail and tamper alerts prevent it |
| Student experience | Anxious, powerless, no information | Can check script status at any time |

---

*Integrated Design Project — Cybersecurity Department, NSUK*
