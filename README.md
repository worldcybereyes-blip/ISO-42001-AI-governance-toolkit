 ISO/IEC 42001:2023 AI Governance & Policy Toolkit

Practical AI Management System (AIMS) governance artifacts translating **ISO/IEC 42001:2023** Clauses 4–10 and Annex A controls into audit-ready templates for enterprise GenAI and agentic AI deployments.

 Repository Contents
- `01_ISO_42001_Statement_of_Applicability.md` — Normative Annex A control selection, inclusion/exclusion justifications, and evidence owners (Clause 6.1.3 f).
- `02_Enterprise_AI_Acceptable_Use_Policy.md` — Workforce & engineering rules for approved LLMs, prohibited data classes, HITL oversight, and incident reporting.

 Framework Alignment
- ISO/IEC 42001:2023: Clauses 4–10 & Annex A (A.2–A.10)
- NIST AI RMF 1.0 & AI 600-1: GOVERN (GV), MAP (MP), MEASURE (MS), MANAGE (MG)
- Regional Compliance: India Digital Personal Data Protection (DPDP) Act & CERT-In 6-Hour Incident Reporting



 ISO/IEC 42001:2023 AI Governance & Policy Toolkit

Practical AI Management System (AIMS) governance artifacts translating **ISO/IEC 42001:2023** Clauses 4–10 and Annex A controls into audit-ready templates for enterprise GenAI and agentic AI deployments.

 Repository Contents
- `01_ISO_42001_Statement_of_Applicability.md` — Normative Annex A control selection, inclusion/exclusion justifications, and evidence owners (Clause 6.1.3 f).
- `02_Enterprise_AI_Acceptable_Use_Policy.md` — Workforce & engineering rules for approved LLMs, prohibited data classes, HITL oversight, and incident reporting.

 Framework Alignment
- ISO/IEC 42001:2023: Clauses 4–10 & Annex A (A.2–A.10)
- NIST AI RMF 1.0 & AI 600-1: GOVERN (GV), MAP (MP), MEASURE (MS), MANAGE (MG)
- Regional Compliance: India Digital Personal Data Protection (DPDP) Act & CERT-In 6-Hour Incident Reporting



 Enterprise AI Acceptable Use Policy (AUP)

Policy ID:** POL-AI-001 | Aligned To: ISO/IEC 42001:2023 (A.2, A.9), NIST AI RMF (GV-1.1), India DPDP Act  

 1. Purpose & Scope
This policy governs the safe, compliant use of Generative AI (GenAI), Large Language Models (LLMs), and autonomous AI agents by all employees, contractors, and engineering teams.

 2. Approved vs. Prohibited Use
- Approved Tools: Only organization-sanctioned LLM endpoints operating under an enterprise Zero-Data-Retention (ZDR) Data Processing Agreement (DPA).
- Prohibited Data Inputs: Never input unredacted PII, customer financial records, source-code secrets, API keys, or regulated health data into public/unapproved AI tools.
- Prohibited Autonomous Actions: AI agents must never execute irreversible production changes (e.g., IAM account deletion, firewall rule drops, or fund transfers) without a verified Human-in-the-Loop (HITL) approval gate.

 3. Security & Integrity Controls
- All external or untrusted inputs (emails, SIEM logs, web scrapes) passed to LLM agents must undergo prompt-injection sanitization (OWASP LLM01 / MITRE ATLAS AML.T0051).
- AI-generated code, compliance mappings, and security triage recommendations must be human-reviewed before production merge or external submission.

 4. Incident Reporting & Enforcement
Suspected data leakage, jailbreaks, or unauthorized agent actions must be reported immediately to the Security Operations / GRC team to meet internal SLA and **CERT-In 6-hour** incident reporting obligations where applicable.
