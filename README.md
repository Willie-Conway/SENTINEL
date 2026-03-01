
# 🛡️ SENTINEL — Insider Threat Detection & Training Platform

![alt text](Screenshots/SENTINEL_Logo.png)

![SENTINEL Platform](https://img.shields.io/badge/SENTINEL-Insider_Threat_Platform-ff6b35?style=for-the-badge&logo=security&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![UEBA](https://img.shields.io/badge/UEBA-User_Behavior_Analytics-8b5cf6?style=for-the-badge&logo=analytics&logoColor=white)

<p align="center">
  <img src="https://img.shields.io/badge/STATUS-LIVE-ff6b35?style=for-the-badge&labelColor=050810" />
  <img src="https://img.shields.io/badge/MONITORED_USERS-152-fbbf24?style=for-the-badge&labelColor=050810" />
  <img src="https://img.shields.io/badge/IOCs-23-10b981?style=for-the-badge&labelColor=050810" />
  <img src="https://img.shields.io/badge/SIMULATIONS-5-3b82f6?style=for-the-badge&labelColor=050810" />
</p>

---

## 🎯 **Project Overview**
SENTINEL is an interactive insider threat detection and training platform designed to simulate real-world cybersecurity scenarios. Built with **HTML, CSS, and JavaScript**, this tool provides a hands-on learning experience for security professionals and analysts. 

## ✨ Key Features

### 🏢 **5 Interactive Modules**

| Module                             | Focus                | Description                                                                       |
| ---------------------------------- | -------------------- | --------------------------------------------------------------------------------- |
| **01 — Dashboard**          | Real-Time Monitoring | Live activity feed, risk scores, anomaly tracking across 152 users                |
| **02 — Behavior Analytics** | UEBA Profiling       | Deep-dive user profiles with risk scoring, timeline analysis, and IOC correlation |
| **03 — Simulations**        | Decision Training    | 5 realistic insider threat scenarios with branching decisions and debriefs        |
| **04 — Indicators Library** | IOC Reference        | 23 behavioral, technical, contextual, and access indicators with severity ratings |
| **05 — Policy Reference**   | Compliance Framework | Key insider threat policies, response procedures, and legal frameworks            |

---

## 📊 **Module 01: Threat Dashboard**

### **Real-Time KPIs** 📈

| KPI                            | Value      | Trend                 |
| ------------------------------ | ---------- | --------------------- |
| **Active Risk Subjects** | 3 Critical | ↑ 2 from yesterday   |
| **Anomalies (24h)**      | 47         | ↑ 12% above baseline |
| **Data Exfil Attempts**  | 9          | 3 blocked by DLP      |
| **Privilege Violations** | 2          | All contained         |

### **Live Activity Feed** ⚡

- **Real-time alerts** with severity badges (CRITICAL/HIGH/MEDIUM/NORMAL)
- **Timestamped events** with detailed metadata
- **Color-coded severity indicators**:
  - 🔴 **CRITICAL** — Immediate action required
  - 🟠 **HIGH** — Escalate to management
  - 🟡 **MEDIUM** — Investigate within 24h
  - 🟢 **NORMAL** — Routine monitoring

### **Sample Feed Events**

| Time     | Event                                         | Severity    |
| -------- | --------------------------------------------- | ----------- |
| just now | Marcus Webb exported 4.8 GB database file     | 🔴 CRITICAL |
| 4m ago   | DLP blocked Sandra Osei email with attachment | 🟠 HIGH     |
| 11m ago  | Jason Tremblay disabled audit logging         | 🔴 CRITICAL |
| 23m ago  | David Achebe: abnormal CRM export volume      | 🟡 MEDIUM   |

### **High-Risk Subjects** 🚨

- **5 top-risk employees** displayed with:
  - Risk score (0-100)
  - Risk level (CRITICAL/HIGH/MEDIUM/LOW)
  - Visual risk bar
  - Click to view full analytics profile

### **Weekly Anomaly Chart** 📊

- **7-day trend** with stacked categories:
  - 🔴 **Exfiltration** — Data theft attempts
  - 🟠 **Access Abuse** — Unauthorized access
  - 🟡 **Policy Violation** — Policy breaches
  - 🔵 **Credential Anomaly** — Suspicious auth patterns

![alt text](<Screenshots/Threat Dashboard.png>)


---

## 👤 **Module 02: Behavior Analytics**

### **5 Employee Profiles** 🧑‍💼

| Employee                 | Role               | Risk Level  | Score | Key Indicators                                                     |
| ------------------------ | ------------------ | ----------- | ----- | ------------------------------------------------------------------ |
| **Marcus Webb**    | Sr. Database Admin | 🔴 CRITICAL | 87    | Mass database exports, USB activity, HR access, resignation notice |
| **Sandra Osei**    | Financial Analyst  | 🟠 HIGH     | 72    | Personal email exfiltration, excessive printing, failed logins     |
| **Jason Tremblay** | DevOps Engineer    | 🟠 HIGH     | 61    | CloudTrail disabled, repo cloning, credential access               |
| **David Achebe**   | Sales Manager      | 🟡 MEDIUM   | 33    | CRM export spike, competitor research                              |
| **Priya Nair**     | HR Specialist      | 🟢 LOW      | 18    | Minor offboarding access                                           |

### **Profile Features** 📋

- **Risk score** (0-100) with color-coded level
- **Access tier** and tenure information
- **Anomaly count** (30-day window)
- **Data access volume** and off-hours login stats
- **Active indicators** list with detailed IOCs
- **Timeline view** of recent activity with flag severity

### **Timeline Activity** ⏱️

Each timeline entry includes:

- Timestamp
- Event description
- Technical detail
- Severity flag (CRITICAL/HIGH/MEDIUM/NORMAL)
- Color-coded line for visual tracking

### **Sample Timeline Entries**

```
02:14 AM — Large SQL dump exported · customer_data.sql · 4.8 GB 🔴 CRITICAL
11:45 PM — VPN access from new geo-location · Chicago IL (home: Dallas TX) 🟠 HIGH
07:45 PM — Email to personal account flagged by DLP · Q4_Projections_Final.xlsx 🟠 HIGH
```

![alt text](<Screenshots/Behavior Analytics.png>)

---

## 🎮 **Module 03: Insider Threat Simulations**

### **5 Realistic Scenarios** 🕵️

| Scenario                           | Difficulty | Type               | Time    | Description                                                                           |
| ---------------------------------- | ---------- | ------------------ | ------- | ------------------------------------------------------------------------------------- |
| **The Departing Admin**      | 🔴 HARD    | Data Exfiltration  | ~12 min | Privileged admin in notice period exports 4.8 GB database — malicious or legitimate? |
| **The Disgruntled Analyst**  | 🟠 MEDIUM  | Data Leakage       | ~8 min  | Analyst after negative review attempts email exfiltration and excessive printing      |
| **The Credential Harvester** | 🔴 HARD    | Privilege Abuse    | ~10 min | DevOps engineer disables audit logging, accesses credentials, clones private repos    |
| **The Unwitting Accomplice** | 🟢 EASY    | Social Engineering | ~7 min  | Employee shares credentials with coworker who accesses unauthorized HR data           |
| **The Shadow IT Operator**   | 🟠 MEDIUM  | Policy Evasion     | ~8 min  | Sales manager uses unauthorized cloud storage and messaging apps                      |

### **Simulation Features** 🎯

- **Multi-scene narratives** (3-4 scenes per simulation)
- **Evidence panels** with 6+ data points per scene
- **Multiple-choice decisions** with letter indicators (A/B/C/D)
- **Immediate feedback** explaining why choices are correct/incorrect
- **Detailed debrief** with score and performance grade
- **Score tracking** (X/4, X/3 correct)

### **Sample Decision Points**

```
SCENE 01: 02:14 AM — Marcus Webb exported 4.8 GB SQL file from production database. 
He's in his 2-week notice period. What is your FIRST response?

[A] Immediately lock Marcus's account and escalate to management and legal
[B] Flag the alert, check for approved tickets, and monitor further ✓
[C] Email Marcus asking him to explain the export
[D] Delete the exported file from the server remotely
```

### **Debrief Grades** 🏆

| Score | Grade        | Color     |
| ----- | ------------ | --------- |
| 100%  | EXPERT       | 🟢 Green  |
| ≥75% | PROFICIENT   | 🔵 Cyan   |
| ≥50% | DEVELOPING   | 🟡 Yellow |
| <50%  | NEEDS REVIEW | 🔴 Red    |

![alt text](<Screenshots/Training Simulations.png>)

![alt text](<Screenshots/The Unwitting Accomplice.png>)
---


## 📚 **Module 04: Indicators Library**

### **23 IOCs Across 4 Categories** 🔍

| Category             | Indicators | Description                                                                                         |
| -------------------- | ---------- | --------------------------------------------------------------------------------------------------- |
| **Technical**  | 8          | Mass data export, audit log tampering, USB devices, concurrent sessions, DLP triggers               |
| **Behavioral** | 6          | Triggering life events, resignation, out-of-scope access, expressed grievances, competitor research |
| **Contextual** | 4          | Financial distress, failed clearance, conflicts, pre-announcement resignation                       |
| **Access**     | 5          | Privilege creep, service account misuse, credential sharing                                         |

### **Severity Ratings** ⚠️

| Severity           | Color     | Count | Examples                                             |
| ------------------ | --------- | ----- | ---------------------------------------------------- |
| **CRITICAL** | 🔴 Red    | 7     | Mass data export, audit log tampering                |
| **HIGH**     | 🟠 Orange | 8     | Resignation, competitor research, credential sharing |
| **MEDIUM**   | 🟡 Yellow | 6     | Excessive printing, privilege creep                  |
| **LOW**      | 🟢 Green  | 2     | Sudden behavior change, conflicts with colleagues    |

### **IOC Details** 📋

Each indicator includes:

- **Name** — Clear identifier
- **Description** — What it looks like in practice
- **Type** — Technical/Behavioral/Contextual/Access
- **Severity** — CRITICAL/HIGH/MEDIUM/LOW
- **Category filter** — Filter by type


![alt text](<Screenshots/Indicators of Compromise.png>)
---

## 📜 **Module 05: Policy Reference**

### **6 Key Policies** 📄

| Policy                                         | Icon | Summary                                       |
| ---------------------------------------------- | ---- | --------------------------------------------- |
| **Data Handling & Classification**       | 📋   | 4 sensitivity tiers, approved storage methods |
| **Acceptable Use Policy (AUP)**          | 💻   | Corporate device use, software restrictions   |
| **Privileged Access Management**         | 🔑   | Just-in-time access, dual-authorization       |
| **Departing Employee Protocol**          | 🚪   | Enhanced monitoring, data return requirements |
| **Insider Threat Response Procedures**   | ⚑   | Legal hold, escalation, covert monitoring     |
| **Incident Reporting & Non-Retaliation** | 🔔   | Anonymous reporting, whistleblower protection |

### **Policy Content** 📖

- **Data Handling** — Public/Internal/Confidential/Restricted tiers
- **PAM Policy** — JIT access, dual-person authorization, session recording
- **Departing Employee** — 24h notification, access review, forensic imaging
- **Response Procedures** — Do not alert, legal hold, covert monitoring

---

## 🎨 **Design & Aesthetics**

### **Security Operations Center (SOC) Dashboard** 🖥️

- **Dark background** (`#050810`) — SOC standard for reduced eye strain
- **Orange primary** (`#ff6b35`) for alerts and critical indicators
- **Grid backgrounds** with subtle radial gradients
- **Professional typography**:
  - **Syne** — Headers, titles, risk scores
  - **JetBrains Mono** — Terminal output, timestamps, technical data

### **Color Coding** 🎨

| Element                   | Color  | Hex         | Usage                  |
| ------------------------- | ------ | ----------- | ---------------------- |
| **CRITICAL**        | Red    | `#f43f5e` | Immediate threats      |
| **HIGH**            | Orange | `#fb923c` | Escalate immediately   |
| **MEDIUM**          | Yellow | `#fbbf24` | Investigate within 24h |
| **LOW**             | Green  | `#10b981` | Routine monitoring     |
| **Technical IOCs**  | Cyan   | `#06b6d4` | Technical indicators   |
| **Behavioral IOCs** | Purple | `#8b5cf6` | Behavioral indicators  |

### **UI Components** 🧩

- **Stat cards** with KPI values and trend indicators
- **Progress bars** for risk scores and completion
- **Activity feed** with timestamped events
- **Profile cards** with avatar and risk level
- **Timeline view** with visual severity indicators
- **Simulation cards** with difficulty badges
- **IOC table** with category filtering


![alt text](<Screenshots/Policy Reference.png>)

---

## 🛠️ **Technical Implementation**

### **Architecture**

```
┌─────────────────────────────────────┐
│        SENTINEL Platform             │
├─────────────────────────────────────┤
│                                     │
│  ┌─────────────────────────────┐   │
│  │   Module 1: Dashboard        │   │
│  │   • KPI cards                │   │
│  │   • Activity feed            │   │
│  │   • Risk list                │   │
│  │   • Weekly chart             │   │
│  └─────────────────────────────┘   │
│                                     │
│  ┌─────────────────────────────┐   │
│  │   Module 2: Analytics        │   │
│  │   • Employee selector        │   │
│  │   • Profile cards            │   │
│  │   • Timeline view            │   │
│  │   • IOC correlation          │   │
│  └─────────────────────────────┘   │
│                                     │
│  ┌─────────────────────────────┐   │
│  │   Module 3: Simulations      │   │
│  │   • 5 scenarios             │   │
│  │   • Scene-based narrative   │   │
│  │   • Decision engine         │   │
│  │   • Debrief system          │   │
│  └─────────────────────────────┘   │
│                                     │
│  ┌─────────────────────────────┐   │
│  │   Module 4: IOCs            │   │
│  │   • 23 indicators           │   │
│  │   • Category filtering      │   │
│  │   • Severity rating         │   │
│  └─────────────────────────────┘   │
│                                     │
│  ┌─────────────────────────────┐   │
│  │   Module 5: Policy           │   │
│  │   • 6 policies              │   │
│  │   • Detailed content        │   │
│  └─────────────────────────────┘   │
└─────────────────────────────────────┘
```

### **Key Functions**

```javascript
// Module 1: Dashboard
renderDashboard()        // Render activity feed, risk list, weekly chart

// Module 2: Analytics
renderAnalytics()        // Render employee selector and profile
selectEmployee(id)       // Switch active employee
renderProfile()          // Display selected employee's profile and timeline

// Module 3: Simulations
renderSimulations()      // Render simulation cards
startSim(simId)          // Launch simulation player
renderScene()            // Render current scene with evidence and choices
checkSimAnswer()         // Validate answer and provide feedback
nextScene()              // Advance to next scene
showDebrief()            // Display final score and performance grade

// Module 4: Indicators
renderIndicators()       // Render IOC table with category filtering

// Module 5: Policy
renderPolicy()           // Render policy reference content

// Navigation
showView(id)             // Switch between modules
```

---

## 📊 **Content Breakdown**

| Module                | Items                                     | Interactions                       | Learning Outcomes                                |
| --------------------- | ----------------------------------------- | ---------------------------------- | ------------------------------------------------ |
| **Dashboard**   | 4 KPI cards, 7 feed items, 5 risk entries | Real-time monitoring               | Understand threat landscape and risk scoring     |
| **Analytics**   | 5 employee profiles, 20+ timeline entries | Profile selection, timeline review | Correlate behavioral indicators with risk scores |
| **Simulations** | 5 scenarios, 16 scenes, 64 choices        | Decision making, feedback review   | Apply response procedures to realistic cases     |
| **Indicators**  | 23 IOCs, 4 categories                     | Category filtering                 | Recognize 23 insider threat indicators           |
| **Policy**      | 6 policies                                | Reference reading                  | Understand legal and compliance frameworks       |

---

## 🎥 **Video Demo Script** (45-60 seconds)

| Time | Scene             | Action                                            |
| ---- | ----------------- | ------------------------------------------------- |
| 0:00 | Dashboard         | Show KPI cards and live activity feed             |
| 0:05 | Risk List         | Click Marcus Webb → Show analytics profile       |
| 0:10 | Analytics         | Scroll through timeline with critical flags       |
| 0:15 | Simulations       | Select "The Departing Admin" → Launch simulation |
| 0:20 | Scene 1           | Show evidence panel (6 data points)               |
| 0:25 | Decision          | Select correct option → Show feedback            |
| 0:30 | Scene Progression | Advance through 4 scenes                          |
| 0:35 | Debrief           | Show score (3/4) and EXPERT grade                 |
| 0:40 | Indicators        | Filter by Technical → Show 8 IOCs                |
| 0:45 | Policy            | Scroll through 6 policies                         |
| 0:50 | Close             | Return to dashboard                               |

---

## 🚦 **Performance**

- **Load Time**: < 2 seconds (zero external dependencies)
- **Memory Usage**: < 45 MB
- **CPU Usage**: Minimal (event-driven)
- **Network**: Zero requests after initial load

---

## 🛡️ **Security Notes**

SENTINEL is a **completely safe** educational platform:

- ✅ No actual user monitoring performed
- ✅ All simulations run in browser memory
- ✅ No data collection or tracking
- ✅ No external dependencies
- ✅ Pure HTML/CSS/JavaScript
- ✅ Educational purposes only — learn insider threat detection

---

## 📝 **License**

MIT License — see LICENSE file for details.

---

## **🙏🏿 Acknowledgments**

- **CERT Insider Threat Center** — Insider threat research and frameworks
- **NIST** — Digital identity guidelines and incident response
- **SEI (Software Engineering Institute)** — Insider threat mitigation
- **SANS Institute** — Security awareness training methodology
- **FBI IC3** — Insider threat case studies and statistics

---

## 📧 **Contact**

- **GitHub Issues**: [Create an issue](https://github.com/Willie-Conway/SENTINEL/issues)
- **Website**: https://willie-conway.github.io/SENTINEL/

---

## 🏁 **Future Enhancements**

- [ ] Add more simulations (10+ total)
- [ ] Include real-time UEBA algorithm simulation
- [ ] Export risk reports as PDF
- [ ] Manager dashboard for department-level risk
- [ ] Integration with SIEM simulation
- [ ] Custom risk scoring weights
- [ ] Compliance mapping (GDPR, HIPAA, PCI)
- [ ] Multi-tenant organization support
- [ ] Historical trend analysis
- [ ] Benchmark comparisons across industry

---

<p align="center">
  <strong>🛡️ SENTINEL — Detect, Investigate, and Respond to Insider Threats 🛡️</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/BUILT_WITH-❤️-ff6b35?style=for-the-badge&labelColor=050810" />
  <img src="https://img.shields.io/badge/FOR-SOC_Analysts-3b82f6?style=for-the-badge&labelColor=050810" />
  <img src="https://img.shields.io/badge/TRY_IT_LIVE-10b981?style=for-the-badge&labelColor=050810" />
</p>

---

*Last updated: March 2025*
