# SYSTEM HUMAN // Automated AP & Vendor Leak Detection Engine

An enterprise document audit pipeline built with **Langflow** and **Gemini 3.7 Flash**. Ingests unstructured multi-page supplier invoices, receipts, and health reports, cross-checks arithmetic, evaluates warranty clawback exposure, and flags operational discrepancies in under 15 seconds.

---

## System Architecture

[Raw Multi-Page PDF]
│
▼
┌──────────────────┐
│  File Loader     │ ➔ Extracts unstructured text & raw tabular data
└────────┬─────────┘
│
▼
┌──────────────────┐
│ Gemini 3.7 Flash │ ➔ Ingests SYSTEM HUMAN 3-Part Diagnostic Framework
└────────┬─────────┘
│
▼
┌──────────────────┐
│ Structured Audit │ ➔ 1. Executive Summary
│ Output Stream    │   2. Financial & Physical Anomalies
└──────────────────┘   3. Recovery Action Plan


---

## Live Diagnostic Case Study

* **Input Data:** 2-page vendor billing & vehicle health report (Halfords Autocentres A099).
* **Execution Time:** ~12 seconds.
* **Audit Breakdown:**
  * **Zero Net Overcharge Verification:** Confirmed full 100% credit offset (£195.99) against warranty claim.
  * **Risk Flag (Clawback Exposure):** Flagged replaced tyre at 5.5mm tread depth (61% remaining life), noting audit risk without attached photographic evidence of sidewall failure.
  * **System Logic Glitch:** Flagged automated POS error registering next service due date identically to invoice date.

---

## Output Framework


EXECUTIVE SUMMARY
• Vendor Name & Metadata
• Net vs. Gross Billed Reconciliation
• Scope of Line Items

FINANCIAL ANOMALIES & OPERATIONAL RISKS
• Direct Line-Item Overcharges
• Warranty & Contract Policy Threshold Violations
• Physical Inspection & Asymmetric Wear Risks

RECOVERY ACTION PLAN
• Immediate Remediation Steps
• Evidence Archival (Clawback Protection)
• Vendor System Record Corrections


---

## How to Deploy & Run

1. Clone this repository:
   ```bash
   git clone [https://github.com/SystemHumanAI/vendor-invoice-auditor.git](https://github.com/SystemHumanAI/vendor-invoice-auditor.git)


   Import vendor-invoice-auditor.json directly into your local or cloud Langflow instance.

Supply your Google Gemini API Key in the Language Model node.

Upload any vendor PDF to the Read File node and run the flow.

© SYSTEM HUMAN — Operational AI Systems Architecture

