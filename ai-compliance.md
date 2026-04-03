# AI Compliance Deep Dive — Kenya

*Reference file for the kenya-legal-compliance skill. Load when user asks specifically about AI product compliance.*

## The AI Bill 2026 — Current Status

- **Introduced**: March 2026, before the Senate by Nominated Senator Karen Nyamu
- **Status**: Under Senate review (not yet enacted)
- **Legal momentum**: High Court of Kenya order (February 6, 2026) demanded action on AI regulation
- **Senate directive**: Ministry of ICT ordered to develop national AI policy (March 12, 2026)
- **Review cadence**: Law will be reviewed every 3 years (technology evolves faster than legislation)

**Until the Bill passes**: The Data Protection Act 2019, Computer Misuse and Cybercrimes Act 2018, and Consumer Protection Act 2012 apply to AI products.

---

## Risk Classification Deep Dive

### Determining Your Risk Tier

Answer these questions to classify your AI system:

**Is it prohibited (unacceptable risk)?**
- Does it manipulate users without their awareness?
- Does it exploit vulnerable groups (children, elderly, disabled)?
- Does it enable mass surveillance of citizens?
- Does it perform social scoring by government?
→ If yes to any: **DO NOT BUILD**

**Is it high risk?**
Does your AI make or significantly influence decisions in:
- Health: diagnosis, medication recommendations, treatment plans
- Finance: creditworthiness, insurance risk, fraud classification, loan approvals
- Education: grading, admissions, student performance assessment
- Employment: CV screening, interview scoring, performance review
- Law enforcement / security: risk profiling, surveillance
- Public administration: benefit eligibility, permit approval
→ If yes: **HIGH RISK — see requirements below**

**Is it limited risk?**
- Chatbots and conversational AI
- Recommendation engines (content, products)
- Generative AI tools (text, image, audio, video generation)
- Emotion recognition systems
→ **LIMITED RISK — transparency obligations apply**

**Otherwise**: Minimal risk. Follow DPA + consumer protection.

---

## High-Risk AI — Full Requirements Checklist

### Before Deployment
- [ ] **Human Rights Impact Assessment (HRIA)** — document potential harms to users
- [ ] **Risk Assessment** — identify, evaluate, and mitigate risks
- [ ] **Training data documentation** — sources, consent basis, quality measures
- [ ] **Performance metrics** — accuracy, fairness, bias testing across demographics
- [ ] **Technical documentation** — architecture, training methodology, limitations
- [ ] **Human oversight design** — who can override the system, under what conditions

### At Deployment
- [ ] **Operational logs** — maintain for minimum **5 years** (performance data, decision outputs)
- [ ] **User transparency notice** — inform users an AI system is making decisions about them
- [ ] **Human review mechanism** — users must be able to request human review
- [ ] **Appeals process** — users can challenge AI-driven decisions
- [ ] **Workforce impact assessment** (if AI affects employment at your company or users' companies)
- [ ] **Reskilling programs** — for any jobs displaced by your AI

### Ongoing
- [ ] Quarterly bias and fairness audits
- [ ] Performance monitoring and drift detection
- [ ] Incident reporting to future AI Commissioner
- [ ] Annual documentation review
- [ ] Prepare for regulatory sandbox participation if requested

---

## Limited Risk AI — Requirements Checklist

### Chatbots / Conversational AI
- [ ] Clear disclosure: "You are talking to an AI" at start of every conversation
- [ ] Option to speak with a human (if human alternative exists)
- [ ] Do not impersonate a specific living person
- [ ] Do not claim to be a licensed professional (doctor, lawyer, financial advisor)

### Generative AI (Text, Image, Audio, Video)
- [ ] Label AI-generated content clearly
- [ ] For synthetic media involving real people: obtain explicit written consent
- [ ] Deepfake disclosure required before deployment
- [ ] Do not generate synthetic media that could harm, defame, or harass individuals

### Recommendation Systems
- [ ] Disclose that content is algorithmically recommended
- [ ] Provide a non-personalised alternative if possible
- [ ] Do not recommend harmful content to vulnerable users

---

## AI + Data Protection Intersection

Every AI system processing personal data must comply with DPA 2019:

| AI Activity | DPA Obligation |
|---|---|
| Training on user data | Lawful basis + consent where required |
| Storing training datasets | Purpose limitation + data minimisation |
| Running inference on user queries | Transparency + security |
| Profiling users | Right to object + human review |
| Automated decision-making | Right to explanation + challenge |
| Sharing model outputs with third parties | Data sharing agreements |
| Cross-border model hosting | Transfer safeguards |

**Data Protection Impact Assessment (DPIA)** is required before:
- Deploying any high-risk AI system
- Large-scale profiling of individuals
- Processing biometric or health data with AI
- Using AI for employment or financial decisions

---

## AI in Specific Kenyan Sectors

### AI in Healthcare (Healthtech)
- Follow ODPC Guidance Note on Processing of Health Data
- Health data is **sensitive personal data** — stricter consent requirements
- Any diagnostic AI is high-risk → full HRIA required
- Partner with licensed medical practitioners for clinical AI tools
- mHealth apps: comply with both DPA and forthcoming health data guidelines

### AI in Finance (Fintech AI)
- Credit scoring AI = high risk → HRIA + CBK awareness
- Fraud detection AI = high risk → operational logs required
- DCP Regulations apply if AI is used in digital lending decisions
- Customers must be able to request human review of credit decisions
- ODPC Guidance Note for Digital Credit Providers applies

### AI in Agriculture / Public Services
- Lower risk generally, but monitor for bias affecting marginalized communities
- If used in government benefit allocation → high risk classification

---

## National AI Strategy 2025–2030 Alignment

The Strategy's six pillars create opportunities for builders:

| Pillar | Builder Opportunity | Compliance Note |
|---|---|---|
| AI Digital Infrastructure | Cloud/infrastructure startups | Standard DPA + CMCA |
| Data Research & Development | Data platforms, open datasets | DPA consent + licensing |
| Talent | EdTech AI tools | If grading/assessment → high risk |
| Governance | RegTech, compliance tools | Align with AI Commissioner framework |
| Investment | AI startups seeking funding | ESG + compliance = investor confidence |
| Ethics, Equity & Inclusion | Fairness auditing tools | Align with HRIA requirements |

---

## Preparing for the AI Commissioner

When the AI Bill passes, expect to:
1. **Register** your AI system with the Office of the AI Commissioner
2. **Submit documentation** (risk tier, HRIA, technical docs)
3. **Participate in conformity audits** for high-risk systems
4. **Use regulatory sandbox** for novel/uncertain-risk AI systems
5. **Handle complaints** through Commissioner's complaints process
6. **Respond to algorithmic bias** complaints within defined timelines

**Start building your documentation now** — it will be required at registration.

---

## Common AI Compliance Mistakes to Avoid

❌ **Deploying a high-risk AI without an HRIA** — most common compliance gap  
❌ **No logging** — you won't be able to audit or defend decisions  
❌ **Claiming AI is a licensed professional** — legal liability  
❌ **Not disclosing AI in your product** — violates transparency requirements  
❌ **Using personal data for AI training without lawful basis** — DPA violation  
❌ **No human override mechanism** — required for high-risk systems  
❌ **Assuming the AI Bill doesn't apply yet** — DPA already covers AI data processing  
