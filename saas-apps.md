# General SaaS & App Compliance — Kenya

*Reference file for the kenya-legal-compliance skill. Load when user is building a general app, SaaS product, or consumer-facing digital service.*

## The Minimum Viable Compliance Stack

Every Kenyan app needs these, no exceptions:

### 1. Business Registration
- **Certificate of Incorporation** — Companies Registry (eCitizen)
- **Business Single Permit** — from your county government
- **KRA PIN** — Kenya Revenue Authority
- **NSSF & NHIF** — if you have employees

### 2. Legal Documents
- **Privacy Policy** — required by DPA 2019 (see SKILL.md for checklist)
- **Terms of Service** — protects you and sets user expectations
- **Cookie Policy** — if you use cookies / tracking pixels
- **EULA** — if distributing software

### 3. Data Compliance
- **ODPC Registration** — if processing personal data (most apps do)
- **Consent mechanisms** — opt-in flows that are explicit and withdrawable
- **Data breach response plan** — documented and tested

---

## App Store Compliance

### Google Play Store
- Privacy policy URL required for all apps
- Data safety section requires you to declare what data you collect
- For apps targeting children: strict content + data collection limits
- GDPR compliance may be required for users in EU (even if you're in Kenya)

### Apple App Store
- Privacy nutrition labels required
- App Privacy policy required
- App Tracking Transparency (ATT) framework for tracking across apps

**Kenyan-specific note**: Your privacy policy must satisfy both the App Store requirements AND Kenya's DPA 2019. Write it to the higher standard (DPA is the priority).

---

## Consent Best Practices

### What Counts as Valid Consent Under DPA
- **Freely given** — no coercion, no bundled consent for unrelated purposes
- **Specific** — separate consent for each data use purpose
- **Informed** — clear plain-language explanation of what you'll do with data
- **Unambiguous** — an active action (tick box, button press) — NOT pre-ticked boxes
- **Withdrawable** — user can withdraw consent as easily as they gave it

### Consent UI Patterns

✅ **Good**:
- "I agree to receive marketing emails" (unchecked by default)
- "Share my usage data to improve the app" (separate toggle, default OFF)
- Granular consent screen with individual toggles per purpose

❌ **Bad**:
- Pre-ticked checkboxes
- "By using this app you agree to all our data practices" buried in ToS
- Bundling marketing consent with essential service sign-up
- Dark patterns that make it harder to decline than accept

---

## Push Notifications & Direct Marketing

**Law**: DPA 2019 + Consumer Protection Act 2012

- Obtain explicit opt-in consent **before** sending marketing notifications
- Every marketing message must have an **unsubscribe** mechanism
- Honor unsubscribe requests within reasonable time
- Do not send unsolicited commercial messages (could constitute cyber harassment under CMCA)
- SMS marketing: follow Communications Authority of Kenya guidelines

---

## Third-Party Integrations & Data Sharing

When integrating SDKs, analytics, or third-party services:

**You remain responsible** for what third parties do with your users' data.

Required actions:
- [ ] Review privacy practices of every SDK/third-party you integrate
- [ ] Declare all third-party data sharing in your Privacy Policy
- [ ] Enter Data Processing Agreements (DPAs) with processors
- [ ] Ensure cross-border transfer safeguards for overseas services (AWS, Google, Firebase, etc.)
- [ ] Audit third-party integrations quarterly

**Common risky integrations**:
- Analytics (Firebase, Mixpanel, Amplitude) — declare data sharing
- Advertising SDKs (Meta, Google Ads) — explicit consent required
- Customer support tools (Intercom, Zendesk) — DPA with vendor required
- Payment processors (Stripe, Flutterwave, Pesapal) — limited data sharing okay

---

## Children & Minor Users

If your app could be used by people under 18:

**DPA 2019 + Children's Act (Cap 141)**:
- Children's data requires **parental/guardian consent**
- Age verification required before processing children's data
- Cannot target marketing at children
- No profiling of children
- Enhanced data minimisation for children's data

**Design principle**: If there's any chance minors use your app, build age verification and parental consent flows.

---

## Employee & HR Data

If you build HR tech or process employee data:

- Employment Act 2007 governs workplace data
- DPA applies to employee personal data
- Cannot monitor employees without disclosure and legal basis
- Background checks require explicit employee consent
- Employee data cannot be shared without consent (except legal requirements)

---

## Open Source & Intellectual Property

**Computer Misuse and Cybercrimes Act 2018 + Copyright Act Cap 130**:

- Clearly license your open source code (MIT, Apache, GPL etc.)
- Do not include GPL-licensed code in proprietary products without compliance
- Respect patent claims (limited patent activity in Kenya currently)
- Brand names and logos: trademark registration at KEPI (Kenya Intellectual Property Institute)
- AI-generated code: currently no specific Kenya guidance — document provenance

---

## Accessibility

No mandatory accessibility law yet in Kenya for apps, but:
- Disability Act (Cap 133) creates general non-discrimination obligations
- Best practice: Follow WCAG 2.1 AA guidelines
- Government procurement increasingly requires accessibility compliance
- Demonstrates good faith and widens your addressable market

---

## B2B SaaS — Additional Obligations

If selling software to Kenyan businesses or government:

**Government procurement**: Follow Public Procurement and Asset Disposal Act 2015
- Registration with Public Procurement Regulatory Authority (PPRA) may be required
- Data sovereignty requirements — government data may require local hosting
- Security clearances for certain government data categories

**Enterprise data processing**:
- Data Processing Agreements required with all B2B customers
- Sub-processor management and notification obligations
- Audit rights must be contractually available to customers

---

## Incident Response Template

When a data breach occurs:

**Hour 0–4**: Contain the breach. Identify scope. Do not delete evidence.  
**Hour 4–24**: Internal escalation. Document what was accessed.  
**Hour 24–48**: If you're a data processor, notify your data controller.  
**Hour 48–72**: If you're a data controller, notify ODPC. Assess user notification need.  
**Post-72hrs**: Notify affected users if real risk of harm exists. File full incident report with ODPC.

**Notification to ODPC**:
- File at: odpc.go.ke
- Include: Nature of breach, categories of data affected, approximate number of individuals, likely consequences, measures taken

---

## Useful Templates & Tools

| Resource | Where to Find |
|---|---|
| ODPC Registration | odpc.go.ke |
| Privacy policy generator (Kenya) | Use as starting point, customise for your product |
| DPA full text | kenyalaw.org |
| CMCA full text | kenyalaw.org |
| CBK regulations | centralbank.go.ke |
| KRA tax registration | kra.go.ke |
| Business registration | ecitizen.go.ke |
