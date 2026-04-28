# ATO Security Package
## Authorization to Operate — MedCore Electronic Health Records Platform (EHRP)

**System:** MedCore Electronic Health Records Platform (EHRP)
**Organization:** MedCore Health Systems (Fictional)
**Classification:** MODERATE (FIPS 199)
**Framework:** NIST SP 800-37 Rev 2 | NIST SP 800-53 Rev 5 | FedRAMP Moderate Baseline
**Status:** In Development

> **Disclaimer:** This is a fictional ATO security package created for cybersecurity portfolio demonstration purposes. All content, systems, personnel, and data are fabricated. This does not represent any real organization, real system, or real authorization package.
>
> ---
>
> ## Overview
>
> This repository contains a complete Authorization to Operate (ATO) Security Package for the MedCore EHRP, built following the NIST Risk Management Framework (RMF) Steps 0–6 and structured to meet FedRAMP Moderate baseline requirements. The package includes a full System Security Plan (SSP), all supporting artifacts, all 20 NIST SP 800-53 Rev 5 control family implementations, and all required FedRAMP SSP attachments.
>
> An ATO is the official authorization granted by a designated Authorizing Official (AO) that permits a system to operate within an acceptable risk threshold. This package documents every component of that authorization process.
>
> ---
>
> ## NIST RMF Process Summary
>
> | Step | Name | Purpose | Status |
> |------|------|---------|--------|
> | **Step 0** | Prepare | Establish roles, governance, and organizational risk strategy | Complete |
> | **Step 1** | Categorize | Classify system using FIPS 199 and NIST SP 800-60 | Complete |
> | **Step 2** | Select | Choose security control baseline from NIST SP 800-53 | Complete |
> | **Step 3** | Implement | Deploy and document security controls | In Progress |
> | **Step 4** | Assess | Evaluate control effectiveness via Security Assessment | Planned |
> | **Step 5** | Authorize | Authorizing Official reviews risk and issues ATO/IATO | Planned |
> | **Step 6** | Monitor | Continuous monitoring, POA&M management, annual assessments | Planned |
>
> ---
>
> ## Repository Structure
>
> ```
> ato-security-package/
> ├── README.md                              ← This document
> │
> ├── 00-rmf-preparation/
> │   ├── roles-and-responsibilities.md      ← RMF roles: AO, ISSO, SCA, SysOwner
> │   ├── risk-management-strategy.md        ← Organizational risk tolerance and strategy
> │   └── common-control-identification.md   ← Inherited vs. system-specific controls
> │
> ├── 01-categorization/
> │   ├── fips-199-worksheet.md              ← Security categorization (C/I/A)
> │   ├── nist-800-60-mapping.md             ← Information type mappings
> │   └── system-categorization-memo.md      ← Official categorization determination
> │
> ├── 02-control-selection/
> │   ├── control-baseline-selection.md      ← Moderate baseline selection rationale
> │   ├── tailoring-decisions.md             ← Control additions, removals, compensating
> │   └── control-allocation-table.md        ← System vs. common vs. hybrid controls
> │
> ├── 03-system-security-plan/
> │   ├── ssp-main.md                        ← Full System Security Plan narrative
> │   ├── ssp-section-1-information.md       ← System information and overview
> │   ├── ssp-section-2-system-description.md← System description and boundary
> │   ├── ssp-section-3-environment.md       ← Operating environment
> │   ├── ssp-section-4-personnel.md         ← Roles and responsibilities
> │   ├── ssp-section-5-interconnections.md  ← System interconnections
> │   └── ssp-section-6-control-summary.md   ← Control implementation summary
> │
> ├── 04-control-implementations/
> │   ├── AC-Access-Control/
> │   ├── AT-Awareness-Training/
> │   ├── AU-Audit-Accountability/
> │   ├── CA-Assessment-Authorization/
> │   ├── CM-Configuration-Management/
> │   ├── CP-Contingency-Planning/
> │   ├── IA-Identification-Authentication/
> │   ├── IR-Incident-Response/
> │   ├── MA-Maintenance/
> │   ├── MP-Media-Protection/
> │   ├── PE-Physical-Environmental/
> │   ├── PL-Planning/
> │   ├── PM-Program-Management/
> │   ├── PS-Personnel-Security/
> │   ├── PT-PII-Processing-Transparency/
> │   ├── RA-Risk-Assessment/
> │   ├── SA-System-Services-Acquisition/
> │   ├── SC-System-Communications/
> │   ├── SI-System-Information-Integrity/
> │   └── SR-Supply-Chain-Risk/
> │
> ├── 05-fedramp-attachments/
> │   ├── attachment-01-information-security-policies.md
> │   ├── attachment-02-user-guide.md
> │   ├── attachment-03-digital-identity-worksheet.md
> │   ├── attachment-04-privacy-impact-assessment.md
> │   ├── attachment-05-rules-of-behavior.md
> │   ├── attachment-06-information-system-contingency-plan.md
> │   ├── attachment-07-configuration-management-plan.md
> │   ├── attachment-08-incident-response-plan.md
> │   ├── attachment-09-cis-and-csa.md
> │   ├── attachment-10-security-assessment-plan.md
> │   ├── attachment-11-security-assessment-report.md
> │   ├── attachment-12-plan-of-action-milestones.md
> │   └── attachment-13-supply-chain-risk-management-plan.md
> │
> ├── 06-risk-assessment/
> │   ├── risk-assessment-report.md
> │   ├── threat-catalog.md
> │   ├── vulnerability-findings.md
> │   └── risk-register.md
> │
> ├── 07-authorization-decision/
> │   ├── authorization-package-summary.md
> │   ├── security-assessment-report.md
> │   └── authorization-to-operate-memo.md
> │
> ├── 08-continuous-monitoring/
> │   ├── conmon-strategy.md
> │   ├── poam-tracker.md
> │   ├── monthly-reporting-template.md
> │   └── annual-assessment-schedule.md
> │
> └── diagrams/
>     ├── nist-rmf-process-flow
>     ├── system-authorization-boundary
>     ├── control-inheritance-model
>     └── continuous-monitoring-workflow
> ```
>
> ---
>
> ## NIST SP 800-53 Rev 5 — All 20 Control Families
>
> Each control family folder in `04-control-implementations/` contains individual control implementation statements for every applicable control in the MedCore EHRP Moderate baseline.
>
> | ID | Control Family | Controls in Moderate Baseline | Key Focus Areas |
> |----|---------------|------------------------------|----------------|
> | **AC** | Access Control | AC-1 through AC-25 | Least privilege, account management, session controls, remote access |
> | **AT** | Awareness & Training | AT-1 through AT-6 | Security awareness training, role-based training, insider threat |
> | **AU** | Audit & Accountability | AU-1 through AU-16 | Audit logging, log review, audit reduction, time stamps |
> | **CA** | Assessment, Authorization & Monitoring | CA-1 through CA-9 | Security assessments, POA&M, system interconnections |
> | **CM** | Configuration Management | CM-1 through CM-14 | Baseline configurations, change control, software inventory |
> | **CP** | Contingency Planning | CP-1 through CP-13 | BCP/DR, backup procedures, system recovery |
> | **IA** | Identification & Authentication | IA-1 through IA-13 | MFA, password policies, PKI, authenticator management |
> | **IR** | Incident Response | IR-1 through IR-10 | Incident handling, reporting, forensics, monitoring |
> | **MA** | Maintenance | MA-1 through MA-6 | Controlled maintenance, maintenance tools, remote maintenance |
> | **MP** | Media Protection | MP-1 through MP-8 | Media access, marking, storage, transport, sanitization |
> | **PE** | Physical & Environmental | PE-1 through PE-23 | Physical access, facility protection, environmental controls |
> | **PL** | Planning | PL-1 through PL-11 | Security planning, concept of operations, central management |
> | **PM** | Program Management | PM-1 through PM-32 | Enterprise risk management, governance, privacy programs |
> | **PS** | Personnel Security | PS-1 through PS-9 | Screening, termination, transfers, access agreements |
> | **PT** | PII Processing & Transparency | PT-1 through PT-8 | Privacy notices, consent, information sharing, records |
> | **RA** | Risk Assessment | RA-1 through RA-10 | Risk assessment, vulnerability scanning, privacy risk |
> | **SA** | System & Services Acquisition | SA-1 through SA-23 | SDLC, supply chain, developer security, outsourcing |
> | **SC** | System & Communications Protection | SC-1 through SC-51 | Encryption, network segmentation, boundary protection |
> | **SI** | System & Information Integrity | SI-1 through SI-23 | Malware protection, flaw remediation, information accuracy |
> | **SR** | Supply Chain Risk Management | SR-1 through SR-12 | Vendor risk, component authenticity, supply chain controls |
>
> ---
>
> ## FedRAMP SSP Attachments
>
> All 13 required FedRAMP SSP attachments are included in this package under `05-fedramp-attachments/`:
>
> | # | Attachment | Description |
> |---|-----------|-------------|
> | 1 | Information Security Policies and Procedures | Organization-level security policies applicable to the system |
> | 2 | User Guide | End-user operational guide for the EHRP |
> | 3 | Digital Identity Worksheet | NIST SP 800-63 identity assurance level determination |
> | 4 | Privacy Impact Assessment (PIA) | Analysis of PHI/PII handling and privacy risks |
> | 5 | Rules of Behavior (RoB) | Acceptable use and user responsibility acknowledgment |
> | 6 | Information System Contingency Plan (ISCP) | Business continuity and disaster recovery procedures |
> | 7 | Configuration Management Plan (CMP) | Change management and configuration baseline processes |
> | 8 | Incident Response Plan (IRP) | Procedures for detecting, reporting, and responding to incidents |
> | 9 | Control Implementation Summary (CIS) & Customer Responsibility Matrix (CRA) | Control ownership mapping |
> | 10 | Security Assessment Plan (SAP) | Methodology for assessing control effectiveness |
> | 11 | Security Assessment Report (SAR) | Findings from the independent security assessment |
> | 12 | Plan of Action & Milestones (POA&M) | Tracking of open findings and remediation timelines |
> | 13 | Supply Chain Risk Management Plan (SCRMP) | Vendor and third-party risk management |
>
> ---
>
> ## Architecture Diagrams
>
> All diagrams are maintained in **architecturediagram.ai** and referenced throughout this package.
>
> | Diagram | Contents | Referenced In |
> |---------|----------|--------------|
> | **NIST RMF Process Flow** | Step-by-step RMF lifecycle from Prepare through Monitor | SSP Section 1, README |
> | **System Authorization Boundary** | All components within and outside the ATO boundary | SSP Section 2, FedRAMP Attachment 9 |
> | **Control Inheritance Model** | System-specific vs. common vs. hybrid control layers | Control Allocation Table |
> | **Continuous Monitoring Workflow** | Monthly reporting, POA&M, annual assessment cycle | ConMon Strategy |
>
> ---
>
> ## Documents Index
>
> | Document | Location | Purpose |
> |----------|----------|---------|
> | System Security Plan (SSP) | `03-system-security-plan/ssp-main.md` | Primary ATO authorization document |
> | FIPS 199 Categorization | `01-categorization/fips-199-worksheet.md` | System security classification |
> | Risk Assessment Report | `06-risk-assessment/risk-assessment-report.md` | Identified risks and treatment decisions |
> | POA&M Tracker | `08-continuous-monitoring/poam-tracker.md` | Open findings with remediation timelines |
> | ATO Authorization Memo | `07-authorization-decision/authorization-to-operate-memo.md` | Final AO authorization letter |
>
> ---
>
> ## Related Repositories
>
> | Repository | Relationship |
> |-----------|-------------|
> | [medcore-health-systems](https://github.com/kcrozz55/medcore-health-systems) | Baseline system — all ATO content applies to this system |
> | [cybersecurity-portfolio](https://github.com/kcrozz55/cybersecurity-portfolio) | Master portfolio index |
> | [nist-rmf-implementation](https://github.com/kcrozz55/nist-rmf-implementation) | Detailed RMF step-by-step documentation |
> | [vulnerability-management-program](https://github.com/kcrozz55/vulnerability-management-program) | Vulnerability findings feeding into POA&M |
> | [security-policies-procedures](https://github.com/kcrozz55/security-policies-procedures) | Policies referenced in SSP and FedRAMP attachments |
>
> ---

---

## System Diagrams

The following diagrams support this ATO package. All diagrams are maintained in the [medcore-health-systems](https://github.com/kcrozz55/medcore-health-systems) repository and referenced here.

---

### Authorization Boundary Diagram

This diagram defines the official ATO boundary for the MedCore EHRP — the precise scope of this authorization package. The boundary encompasses the API Gateway (TLS Termination), Auth Service (OAuth2/OIDC), Application Layer (Patient Record Service, Clinical Logic Engine), and Data Layer (Primary Database, Immutable Audit Store). Components outside the boundary — Client Tier, Identity Provider, and Health Information Exchange — are external dependencies governed by separate agreements. This diagram is referenced in SSP Section 2 and FedRAMP Attachment 9 (CIS/CRA).

![Authorization Boundary Diagram](https://raw.githubusercontent.com/kcrozz55/medcore-health-systems/main/diagrams/authorization-boundary-diagram.png)

---

### NIST RMF Process Flow

This diagram maps the complete NIST Risk Management Framework lifecycle applied to the MedCore EHRP authorization process. Beginning with Step 0 (Prepare), the RMF Core Cycle flows through Categorization (FIPS 199/SP 800-60), Control Selection (SP 800-53 Moderate Baseline), Implementation (System Security Plan), Assessment (Security Assessment Report), Authorization (Authority to Operate), and Continuous Monitoring. The Artifacts layer identifies the three primary deliverables produced by this process: the SSP, SAR, and POA&M — all of which are documented in this repository.

![NIST RMF Process Flow](https://raw.githubusercontent.com/kcrozz55/medcore-health-systems/main/diagrams/nist-rmf-process-flow.png)

---

*All diagrams are version-controlled and reflect the current authorization posture of the MedCore EHRP.*
> *This ATO package is fictional and created for cybersecurity portfolio demonstration purposes only. No real systems, organizations, or sensitive information are involved.*
