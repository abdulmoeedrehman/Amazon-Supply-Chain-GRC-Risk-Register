# Amazon Supply Chain GRC Risk Register & Interactive Dashboard

## Project Overview
This project is a fully functional, enterprise-ready **Governance, Risk, and Compliance (GRC) Risk Register** and **Power BI Dashboard** modeled around a global logistics and supply chain organization (focused on Amazon's operational environment). 

It is designed as a practical tool for daily compliance monitoring, threat tracking, and executive-level risk reporting. It documents, scores, and tracks **50 high-impact cybersecurity and operational risks** spanning critical infrastructure, third-party vendor ecosystems, cloud computing, and automated warehouse environments.

## Core Features & Automation
* **50 Real-World Risk Scenarios:** Covers actual industry threat vectors from 2023–2026, including third-party software zero-days (e.g., MOVEit data exposure), CI/CD pipeline compromises, state-sponsored edge-device targeting, and OT/IoT warehouse hardware vulnerabilities.
* **Automated Risk Scoring:** Built-in Excel logic using a standard 5×5 Likelihood × Impact matrix that dynamically updates total scores and switches risk ratings (`🔴 Critical`, `🟠 High`, `🟡 Medium`, `🟢 Low`).
* **NIST CSF Framework Mapping:** Every risk is directly mapped to the core functions of the NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover).
* **Interactive Power BI Reporting:** A fully dynamic dashboard connected to the dataset that offers cross-filtering capabilities, automated risk-severity donuts, NIST coverage bar charts, and an operational status tracker.

---

## Methodology & Risk Scoring Matrix

Risks are quantified using a standard industry matrix:
* **Score = Likelihood × Impact** (Scale of 1 to 25)

| Score Range | Rating | Action SLA |
| :--- | :--- | :--- |
| **15 – 25** | 🔴 Critical | Immediate Mitigation (14–30 Days) |
| **10 – 14** | 🟠 High | Priority Action (30–60 Days) |
| **5 – 9** | 🟡 Medium | Managed Tracking (90 Days) |
| **1 – 4** | 🟢 Low | Monitored / Accepted |

### Risk Documentation Structure
To ensure comprehensive governance, every single risk follows a strict structure:
`Cause (Root Condition) ➔ Event (Threat Action) ➔ Business Impact (Operational Consequence)`

---

## Dashboard Preview
<img width="701" height="377" alt="image" src="https://github.com/user-attachments/assets/28f06888-92eb-47d0-9b03-b36110135345" />


## Repository Files
1. **`Amazon_Supply Chain GRC Risk Register.xlsx`**: The master data source containing the 50 detailed risk lines, data validation dropdowns, and an automated summary tab.
2. **`Risk Register Dashboard.pbix`**: The Power BI file containing the interactive data models, color-mapped visualizations, and detailed drill-down matrices.

## How to Use This Project
1. **Operational Tracking:** Open the Excel file to add, modify, or update risks. Use the built-in dropdowns to modify `Status` or adjust `Likelihood/Impact` values as mitigations take effect.
2. **Executive Reporting:** Open the Power BI file and click **Refresh** to instantly pull the new Excel data into the interactive charts for C-suite presentations.
