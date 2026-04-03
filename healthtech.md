# Healthtech & MedTech Compliance — Kenya

*Reference file for the kenya-legal-compliance skill. Load when user is building health, medical, or wellness tech.*

## The Healthtech Regulatory Stack

Health data is **sensitive personal data** under DPA 2019. Stricter rules apply.

### Primary Regulators
| Regulator | Scope |
|---|---|
| ODPC | Health data processing under DPA 2019 |
| Ministry of Health | Health apps, medical devices, clinical tools |
| Pharmacy & Poisons Board | Pharmaceutical tech, telemedicine with prescriptions |
| Kenya Medical Practitioners & Dentists Council (KMPDC) | Platforms involving licensed practitioners |

---

## Health Data = Sensitive Personal Data

Under DPA 2019, health data includes:
- Medical records and diagnoses
- Mental health information
- Genetic data
- Biometric data used for health purposes
- Disability information
- Treatment history

**Higher consent standard**: You need **explicit consent** (not just implied) to process health data. Standard opt-in is not enough — the user must actively and specifically consent to health data processing.

---

## ODPC Guidance Note on Health Data

The ODPC has published specific guidance for:
- Hospitals & clinics
- Laboratories
- Pharmaceutical services
- Health insurance providers
- Health research institutions
- **mHealth applications** (mobile health apps)
- **eHealth platforms**
- Health Management Information Systems (HMIS)

**Key requirements from the guidance**:
- Health data processing requires a lawful basis AND explicit consent
- Data minimisation is critical — collect only what is clinically necessary
- Retention periods must align with medical record-keeping standards
- Access controls: only authorised healthcare personnel should access health data
- Audit trails required for all access to health records

---

## mHealth App Compliance Checklist ✅

- [ ] ODPC registration (mandatory for health data processing)
- [ ] Explicit consent for health data collection (separate from general ToS consent)
- [ ] Clear description of what health data is collected and why
- [ ] Data minimisation — do not collect health data "just in case"
- [ ] Local data storage preference (consider Kenya-based servers)
- [ ] Encryption at rest and in transit (AES-256 minimum recommended)
- [ ] Access logs for all health data access
- [ ] Data breach notification procedure (72-hour ODPC notification)
- [ ] User right to deletion (health data retention limits must be defined)
- [ ] No health data sale or sharing with advertisers
- [ ] If AI-driven diagnosis: High-risk AI classification applies

---

## Telemedicine Platforms

If your platform enables doctors to consult patients remotely:

- Doctors must be registered with KMPDC
- Platform does not replace doctor registration — you facilitate, doctors are responsible clinically
- Prescription issuance: Only licensed practitioners can issue prescriptions
- Records: Must comply with health records retention standards
- Consent: Patient must consent to telemedicine consultation AND data processing separately
- Cross-border: Doctors consulting from outside Kenya face jurisdiction questions

---

## AI in Healthcare = High Risk

Any AI making or influencing clinical decisions:
- Full HRIA (Human Rights Impact Assessment) required
- Clinical validation documentation
- Performance metrics across demographic groups (avoid bias in diagnosis)
- Human clinician must be able to override AI recommendations
- Patients must be informed when AI is involved in their care
- Document which datasets were used for training

---

## Research & Clinical Trials

If your platform collects data for health research:
- Ethics approval required from relevant institutional review board
- Separate informed consent for research data use
- De-identification standards must be met before analysis
- Data sharing with international researchers: DPA cross-border transfer rules apply
- KEMRI involvement may be required for certain research categories

---

## Pharmaceutical & MedTech

- Software as a Medical Device (SaMD): International IEC 62304 standards recommended
- Pharmacy & Poisons Board approval for platforms dispensing medication
- Insurance claims processing: IRA regulations + DPA apply
- Medical devices: Kenya Bureau of Standards (KEBS) product approval required
