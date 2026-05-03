# Trello Instructions — Software Testing
**Project:** Location Based Risk Alert System
**Course:** Software Engineering — AIUB Spring 25-26

---

## Lists (Columns)

> Create these 5 lists in order, left to right.

| # | List Name |
|---|---|
| 1 | 📋 To Do |
| 2 | 🔄 In Progress |
| 3 | 🔍 Under Review |
| 4 | ✅ Done |
| 5 | ❌ Blocked |

---

## Labels

> Create these in Board Settings → Labels before making cards.

| Color | Label Name |
|---|---|
| 🔴 Red | Critical |
| 🟠 Orange | High Priority |
| 🔵 Blue | Medium Priority |
| 🟡 Yellow | Testing |
| 🟢 Green | Documentation |

---

## Cards (All start in 📋 To Do)

| Card Title | Assigned To | Label | Due Date |
|---|---|---|---|
| `[TC_01]` Verify User Registration | Mahe Alam Mahi | 🟠 High | 03/05/2026 |
| `[TC_02]` Verify Login Valid & Invalid | Mahe Alam Mahi | 🟠 High | 03/05/2026 |
| `[TC_03]` Verify Map & Heatmap Load | Mohammed Sadat Ishraq Labib | 🟠 High | 03/05/2026 |
| `[TC_04]` Verify Real-Time GPS Tracking | Mohammed Sadat Ishraq Labib | 🟠 High | 03/05/2026 |
| `[TC_05]` Verify Risk Alert — All 5 Types | Wakil Mahmud Rahat | 🔴 Critical | 03/05/2026 |
| `[TC_06]` Verify Risk Details & Safety Tips | Wakil Mahmud Rahat | 🟠 High | 03/05/2026 |
| `[TC_07]` Verify Historical Data Analysis | Khairul Bashar | 🔵 Medium | 03/05/2026 |
| `[TC_08]` Verify Incident Report + Photo | Khairul Bashar | 🔵 Medium | 03/05/2026 |
| `[TC_09]` Verify Admin Creates All 5 Zones | Mahmudur Rahman Mahid | 🟠 High | 03/05/2026 |
| `[TC_10]` Verify Employee Verifies Incident | Mahmudur Rahman Mahid | 🔵 Medium | 03/05/2026 |
| Compile All 10 TCs into Final Document | All Members | 🟢 Documentation | 04/05/2026 |

---

## Each Card Must Have

- ✅ **Checklist** with steps to write and execute the test case
- 👤 **Member** assigned (see table above)
- 📅 **Due date** set
- 🏷️ **Label** applied from the list above

---

## Card Checklists

### [TC_01] Verify User Registration
- [ ] Write test case using standard template
- [ ] Fill: Test Case ID, Module, Priority, Designed by, Date
- [ ] Write test steps (registration flow)
- [ ] Define test data (name, email, password)
- [ ] Define expected results
- [ ] Execute the test case
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_02] Verify Login Valid & Invalid
- [ ] Write test case using standard template
- [ ] Define Run A (valid) and Run B (invalid) in test steps
- [ ] Execute Run A — verify redirect to map dashboard
- [ ] Execute Run B — verify error message shown
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_03] Verify Map & Heatmap Load
- [ ] Write test case using standard template
- [ ] Set precondition: logged in, GPS active, risk zones in DB
- [ ] Execute: open map, check load time (must be < 3 seconds)
- [ ] Verify overlay colours: Red=Critical, Orange=High, Yellow=Medium, Green=Low
- [ ] Verify zone popup appears on tap
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_04] Verify Real-Time GPS Tracking
- [ ] Write test case using standard template
- [ ] Define initial and moved coordinates as test data
- [ ] Enable tracking, simulate coordinate change
- [ ] Verify marker updates within 5 seconds
- [ ] Test toggle off — verify marker freezes at last position
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_05] Verify Risk Alert — All 5 Types ⚠ CRITICAL
- [ ] Write test case using standard template
- [ ] Configure all 5 risk zones in admin panel before testing
- [ ] Enter Flood zone — verify alert within 5 seconds
- [ ] Enter Crime zone — verify alert within 5 seconds
- [ ] Enter Traffic Accident zone — verify alert within 5 seconds
- [ ] Enter Disease Outbreak zone — verify alert within 5 seconds
- [ ] Enter Political Unrest zone — verify alert within 5 seconds
- [ ] Verify each: push notification + in-app banner + alert tone
- [ ] Record actual results for all 5
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_06] Verify Risk Details & Safety Tips
- [ ] Write test case using standard template
- [ ] Tap each of the 5 alert types and open detail screen
- [ ] Verify: Zone Name, Risk Type badge, Severity, mini-map, date/time shown
- [ ] Verify Flood tips: "Move to higher ground"
- [ ] Verify Crime tips: "Contact police (999)"
- [ ] Verify Traffic tips: "Use alternate route"
- [ ] Verify Disease tips: "Wear a mask, avoid crowds"
- [ ] Verify Political tips: "Stay indoors"
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_07] Verify Historical Data Analysis
- [ ] Write test case using standard template
- [ ] Ensure historical records exist in DB before testing
- [ ] Select: Mirpur, Dhaka as area
- [ ] Set date range: 01/01/2026 – 30/04/2026
- [ ] Verify trend chart displays correct data points
- [ ] Change filter to "Flood Only" — verify list reduces correctly
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_08] Verify Incident Report + Photo
- [ ] Write test case using standard template
- [ ] Fill: title, description, select incident type from dropdown
- [ ] Verify GPS location is auto-filled correctly
- [ ] Attach a JPG photo (under 5MB)
- [ ] Submit the report
- [ ] Verify confirmation message shown
- [ ] Verify report appears in employee queue as Pending
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_09] Verify Admin Creates All 5 Risk Zones
- [ ] Write test case using standard template
- [ ] Log in as Admin
- [ ] Create Flood zone — verify orange heatmap on map
- [ ] Create Crime zone — verify red heatmap on map
- [ ] Create Traffic Accident zone — verify yellow heatmap
- [ ] Create Disease Outbreak zone — verify purple heatmap
- [ ] Create Political Unrest zone — verify pink heatmap
- [ ] Verify users inside new zones receive instant alerts
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### [TC_10] Verify Employee Verifies Incident & Notifies Reporter
- [ ] Write test case using standard template
- [ ] Log in as Employee
- [ ] Open a pending report from the verification queue
- [ ] Review: title, description, GPS on mini-map, photo
- [ ] Click Verify and add a response note
- [ ] Verify report status changes to "Verified"
- [ ] Verify reporter receives push notification
- [ ] Verify action logged with employee ID and timestamp
- [ ] Record actual results
- [ ] Mark status: Pass / Fail
- [ ] Submit to group document

### Compile All 10 TCs into Final Document
- [ ] Collect TC_01 & TC_02 from Mahe Alam Mahi
- [ ] Collect TC_03 & TC_04 from Mohammed Sadat Ishraq Labib
- [ ] Collect TC_05 & TC_06 from Wakil Mahmud Rahat
- [ ] Collect TC_07 & TC_08 from Khairul Bashar
- [ ] Collect TC_09 & TC_10 from Mahmudur Rahman Mahid
- [ ] Verify all use the correct template format
- [ ] Add cover page with all 5 student names and IDs
- [ ] Final review by group leader
- [ ] Submit final document

---

## Card Movement Rules

| Situation | Move card to |
|---|---|
| Starting work on a test case | 🔄 In Progress |
| Written but not yet executed | 🔍 Under Review |
| Executed and result recorded | ✅ Done |
| Waiting for module to be ready | ❌ Blocked |

---

## Screenshot Reminder 📷

Take a screenshot of the Trello board at two points:

| When | Purpose |
|---|---|
| All cards in **📋 To Do** | Initial board evidence |
| All cards in **✅ Done** | Final submission evidence |

> Both screenshots go into **Section 5 (Git Workflow)** of the Project Report as Trello board evidence.
