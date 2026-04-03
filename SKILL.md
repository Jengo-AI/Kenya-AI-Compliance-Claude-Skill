---
name: kenya-legal-compliance
description: >
  Comprehensive Kenya legal compliance guide for software developers, AI builders, fintech founders, and digital product creators. 
  Use this skill whenever a Kenyan builder asks about legal compliance, data privacy, user rights, app policies, 
  terms of service, AI regulations, fintech licensing, cybercrime law, or any legal/regulatory question related to 
  building digital products or AI systems in Kenya. Also trigger for questions about: ODPC registration, 
  Data Protection Act obligations, AI Bill 2026 requirements, CBK licensing for digital lenders, 
  Computer Misuse Act compliance, privacy policies for Kenyan apps, cross-border data transfers, 
  AML/KYC requirements for Kenyan startups, or any "am I compliant?" / "what do I need legally?" questions 
  from Kenyan developers and founders. Even if the user doesn't say "Kenya" explicitly but their context 
  suggests they are building in Kenya, use this skill.
---

# Kenya Legal Compliance for Digital Builders

A practical compliance reference for Kenyan software developers, AI builders, and digital founders. 
This skill covers the four core legal pillars every Kenyan builder must understand.

> **Legal Disclaimer**: This skill provides general legal information, not legal advice. 
> For specific situations, consult a qualified Kenyan advocate.

---

## Quick Start: What Do You Need?

Before diving into specifics, identify your product type:

| Product Type | Primary Laws | Start With |
|---|---|---|
| Any app collecting user data | DPA 2019 | [Data Protection](#1-data-protection-act-2019) |
| AI/ML product | DPA + AI Bill 2026 | [AI Compliance](#2-ai-bill-2026--national-ai-strategy) |
| Fintech / digital lending | CBK regs + DPA + AML | [Fintech](#3-fintech--financial-services-laws) |
| Any software business | CMCA + Consumer Protection | [Cybersecurity](#4-computer-misuse--cybercrimes-act-2018) |
| All of the above | All sections | Read everything |

---

## 1. Data Protection Act 2019 (DPA)

**Regulator**: Office of the Data Protection Commissioner (ODPC) — [odpc.go.ke](https://odpc.go.ke)  
**Penalty**: Up to KES 5M (individuals) or 1% of annual gross turnover

### Who Must Comply?

**Everyone** who collects, stores, or processes personal data about Kenyan residents — regardless of where you are based.

### Mandatory Registration with ODPC

You **must register** as a Data Controller and/or Data Processor before processing personal data. Mandatory sectors (regardless of size):
- Financial services
- Healthcare
- Telecommunications
- Any app collecting sensitive data (biometrics, health, finances)

➡️ **Action**: Register at [odpc.go.ke/registration](https://odpc.go.ke)

### The 8 Core Data Principles (Section 25)

Every piece of personal data you collect must be:
1. **Lawful, fair & transparent** — users must know what you collect and why
2. **Purpose-limited** — only collect for a stated, specific purpose
3. **Data minimised** — collect only what you need
4. **Accurate** — keep data up to date; correct errors when flagged
5. **Storage-limited** — delete data when no longer needed
6. **Integrity & confidentiality** — secure it against breaches
7. **Accountability** — you must be able to prove compliance
8. **Collected directly** — get data from the user directly where possible

### Lawful Bases for Processing

You must have at least one valid reason to process data:
- **Consent** — explicit, informed, and withdrawable at any time
- **Contract** — necessary to deliver your service
- **Legal obligation** — required by law
- **Vital interests** — protect someone's life
- **Public interest** — official authority task
- **Legitimate interests** — your business need, if it doesn't override user rights

### User Rights You Must Support

Build these into your product:
- **Right to access** — user can request all their data (respond within 21 days)
- **Right to rectification** — correct inaccurate data (14 days to respond)
- **Right to erasure** — delete data on request (14 days to respond)
- **Right to data portability** — provide data in a usable format
- **Right to object** — to processing for direct marketing or profiling
- **Right to human review** — challenge automated decisions

### Data Breach Protocol

- **Data Controllers**: Notify ODPC within **72 hours** of discovering a breach
- **Data Processors**: Notify your data controller within **48 hours**
- Notify affected users without undue delay if there is real risk of harm

### Cross-Border Data Transfers

Data may only leave Kenya if the destination country provides **adequate protection** OR you use:
- Contractual safeguards approved by ODPC
- Explicit user consent
- For strategic/national interest data: must be processed **within Kenya** (local server required)

### Privacy Policy Checklist ✅

Your privacy policy must include:
- [ ] Identity and contact details of your company
- [ ] What data you collect and why
- [ ] Legal basis for each processing activity
- [ ] How long you retain data
- [ ] Who you share data with (third parties, processors)
- [ ] User rights and how to exercise them
- [ ] Data breach notification procedures
- [ ] Cross-border transfer details if applicable
- [ ] DPO contact details (if you have one)

### When Do You Need a Data Protection Officer (DPO)?

Appoint a DPO if your core activities involve:
- Large-scale processing of sensitive personal data
- Systematic monitoring of individuals at scale
- You are a public authority

---

## 2. AI Bill 2026 & National AI Strategy

**Status**: Before the Senate (March 2026) — not yet law, but prepare now  
**Upcoming Regulator**: Office of the Kenya Artificial Intelligence Commissioner  
**Strategy**: National AI Strategy 2025–2030 (launched March 27, 2025)

### The Four-Tier Risk Classification

The AI Bill adopts an EU AI Act-style risk framework. Know your tier:

#### 🔴 Unacceptable Risk — PROHIBITED
AI systems that manipulate behaviour, exploit vulnerabilities, or enable mass surveillance. **Do not build these.**

#### 🟠 High Risk — Strictest Requirements
AI used in:
- **Healthcare** (diagnosis, treatment recommendations)
- **Finance** (credit scoring, loan decisions, fraud detection)
- **Education** (student assessment, admissions)
- **Employment** (hiring, performance evaluation)
- **Public administration** (benefits, permits, policing)
- **Security systems**

**Requirements for High-Risk AI**:
- [ ] Mandatory human rights impact assessment before deployment
- [ ] Risk assessment documentation
- [ ] Maintain operational logs for **minimum 5 years**
- [ ] Human oversight mechanisms (decisions must be reviewable/overrideable)
- [ ] Transparency disclosures to users
- [ ] Workforce impact assessment if AI affects employment
- [ ] Reskilling/mitigation programs for displaced workers

#### 🟡 Limited Risk — Transparency Requirements
Chatbots, recommendation systems, content generators.

**Requirements**:
- [ ] Notify users they are interacting with an AI system
- [ ] Label AI-generated content (deepfakes, synthetic media)
- [ ] Obtain **clear consent** before deploying synthetic media

#### 🟢 Minimal Risk — Baseline Only
Spam filters, AI in games, basic automation.

**Requirements**: Comply with general DPA and consumer protection laws.

### AI + Data Governance

The AI Bill requires:
- Maintain detailed records of **training datasets**
- Record performance metrics and testing results
- Full compliance with the **Data Protection Act 2019**
- Bias monitoring and algorithmic fairness documentation

### Citizen Rights Under AI Systems

Citizens will gain the right to:
- Human review of automated decisions affecting: employment screening, loan approvals, welfare support, insurance
- Challenge AI-driven outcomes
- Have their views heard before final AI decisions

### Practical Steps: AI Compliance Checklist ✅

- [ ] Classify your AI system by risk tier
- [ ] Document your training data sources and consent basis
- [ ] Build human override mechanisms for consequential decisions
- [ ] Add AI disclosure notices to your UI
- [ ] Register with ODPC (AI processing = personal data processing)
- [ ] Prepare for AI Commissioner registration when the Bill passes
- [ ] Review every 3 years (the law mandates this review cadence)

---

## 3. Fintech & Financial Services Laws

Kenya's fintech regulatory landscape is multi-layered. Navigate it by product type.

### Primary Regulators

| Regulator | What They Oversee |
|---|---|
| **Central Bank of Kenya (CBK)** | Digital lending, mobile money, payment services, remittances |
| **Capital Markets Authority (CMA)** | Investment platforms, securities, crypto (partially) |
| **Insurance Regulatory Authority (IRA)** | Insurtech, embedded insurance |
| **ODPC** | All personal data processing |

### Digital Credit Providers (Digital Lending)

**Law**: CBK (Digital Credit Providers) Regulations 2022 + CBK Amendment Act 2021

**You MUST get a CBK license if** you are providing loans/credit through a digital channel.

**License Requirements**:
- Submit business and financial information to CBK
- Demonstrate source of funds
- Have a business plan reviewed by CBK
- Consumer protection compliance (Part VII of DCPs Regulations)

**Operational requirements**:
- Issue transaction receipts to customers
- Establish customer redress mechanisms
- Observe limits on collection of customer information
- Provide clear terms and conditions
- Get written CBK approval before varying credit terms
- No false advertisements
- Contribute to Credit Reference Bureau (CRB) system

### Mobile Money & Payments

**Law**: Kenya Information and Communications Act (KICA) 1998 + CBK Payment Services Regulations + National Payments Systems Act (NPSA)

- Mobile money regulated by KICA (Communications Authority of Kenya oversees)
- Payment services require CBK authorization
- Follow CBK National Payments Strategy 2022–2025 guidance
- Cybersecurity: Comply with CBK Guidelines on Cybersecurity for Payment Service Providers

### AML/KYC Requirements

**Law**: Proceeds of Crime and Anti-Money Laundering Act (POCAMLA) 2009

All financial services platforms must:
- [ ] Implement Know Your Customer (KYC) procedures
- [ ] Conduct Customer Due Diligence (CDD)
- [ ] Monitor and report suspicious transactions
- [ ] Keep AML transaction records
- [ ] Report cyber attacks/intrusions within **24 hours** to the National Computer and Cybercrimes Co-ordination Committee
- [ ] Follow National Payment System AML Guidelines 2013 (for mobile payments)

### Cryptocurrency & Blockchain

CBK has **not licensed** crypto as legal tender. Current stance:
- No legislative restriction on operating virtual assets
- CBK circulars caution public and banks against dealing with **unlicensed** entities
- Comply with NPSA, CMA, and KICA if your product touches payments
- If classified as collective investment scheme → register with CMA

### Investment Platforms

- Portfolio under KES 10M → licensed as **investment adviser**
- Portfolio over KES 10M → **fund manager license** required
- Register with Capital Markets Authority (CMA)
- CMA Regulatory Sandbox available for 12-month test periods

### Tax Compliance for Fintechs

- **VAT**: 16% on mobile money and digital lending services
- **Corporate Income Tax**: 30% (resident), 37.5% (non-resident)
- Register with Kenya Revenue Authority (KRA)

---

## 4. Computer Misuse & Cybercrimes Act 2018 (CMCA)

**Law**: Computer Misuse and Cybercrimes Act No. 5 of 2018  
**Penalties**: Up to KES 20M and/or imprisonment for serious offences

### What This Law Criminalises

As a developer, do **not** build systems that enable:
- Unauthorised access to computer systems
- Cyber espionage
- Cyber harassment or stalking
- Interception of data without consent
- False publication (misinformation systems)
- Identity theft through computer systems

### Developer Obligations

- **Incident reporting**: Report cyber attacks or intrusions within **24 hours** to the National Computer and Cybercrimes Co-ordination Committee (NC4)
- **Data security**: Implement reasonable technical safeguards
- **No unauthorized access**: Security testing must be authorized (get written permission before penetration testing a system)

### Practical Security Checklist ✅

- [ ] HTTPS/TLS on all endpoints
- [ ] Input validation and sanitization
- [ ] Authentication and authorization controls
- [ ] Audit logs for sensitive operations
- [ ] Incident response plan documented
- [ ] Penetration testing with written authorization
- [ ] Vulnerability disclosure policy published

---

## 5. Consumer Protection Act 2012

Applies to all digital products and services.

**Key obligations**:
- No misleading advertising or false claims about your product
- Disclosure of all fees, charges, and conditions upfront
- Customer complaints mechanism required
- No unconscionable conduct (exploiting user vulnerability)
- For fintech: Disclose if you are NOT a deposit-taking institution
- Honour your terms of service

---

## 6. Terms of Service & Privacy Policy Requirements

### Minimum Terms of Service Must Include:
- Who you are and how to contact you
- What your service does and what it does not do
- User responsibilities and prohibited conduct
- Intellectual property ownership
- Limitation of liability (follow Kenyan contract law)
- Dispute resolution mechanism (specify Kenyan jurisdiction)
- Termination conditions

### For AI Products — Extra Disclosures Required:
- Clearly state when users are interacting with AI
- Accuracy limitations of AI outputs
- That AI is not professional advice (medical, legal, financial)
- How you handle AI-generated content involving users

---

## 7. Sector-Specific Quick References

For detailed guidance by sector, read the relevant reference file:

| Sector | Reference File |
|---|---|
| Healthtech / MedTech | `references/healthtech.md` |
| Fintech / Payments | `references/fintech-deep.md` |
| AI Products | `references/ai-compliance.md` |
| General SaaS / Apps | `references/saas-apps.md` |

---

## 8. Compliance Roadmap for New Kenyan Builders

### Stage 1 — Before Launch (MVP)
1. Register your business (Certificate of Incorporation + Business Permit from county)
2. Determine if you need ODPC registration (most apps do → register)
3. Write a privacy policy aligned with DPA 2019
4. Write terms of service
5. Implement consent mechanisms in your app
6. Set up a data breach response procedure

### Stage 2 — At Launch
1. Ensure all user-facing disclosures are live
2. If fintech: CBK licensing application underway (do not launch digital lending without it)
3. If AI product: Classify your risk tier and document it
4. Enable all user rights features (access, deletion, correction requests)

### Stage 3 — Post-Launch / Scaling
1. Register DPO if required
2. Conduct Data Protection Impact Assessment (DPIA) for high-risk processing
3. Quarterly compliance reviews
4. Monitor AI Bill progress and prepare for Commissioner registration

---

## 9. Key Contacts & Official Resources

| Body | Website | Purpose |
|---|---|---|
| ODPC | odpc.go.ke | Data protection registration & guidance |
| CBK | centralbank.go.ke | Financial services licensing |
| CMA | cma.or.ke | Capital markets & investment licensing |
| CA Kenya | ca.go.ke | Communications & ICT regulations |
| NC4 | nc4.go.ke | Cybercrime reporting |
| Kenya Law | kenyalaw.org | Read all Acts in full |

---

## 10. Penalties at a Glance

| Violation | Maximum Penalty |
|---|---|
| DPA breach (individual) | KES 5,000,000 |
| DPA breach (organisation) | 1% of annual gross turnover |
| DPA general offence | KES 3M or 10 years imprisonment |
| Cybercrime (serious) | KES 20M or imprisonment |
| Unregistered digital lending | CBK license revoked + fines |
| Failure to register with ODPC | Regulatory enforcement |

---

*Last updated: April 2026 | Based on: DPA 2019, AI Bill 2026 (Senate), CMCA 2018, CBK Digital Credit Providers Regulations 2022, POCAMLA 2009, Consumer Protection Act 2012, National AI Strategy 2025–2030*
