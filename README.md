# Agentic Aged Care Explorer

> **A hypothetical, AI-generated interactive framework for exploring how agentic AI workflows could reshape roles, decisions, and care delivery in residential aged care — and what that thinking means for any industry.**

[![Apache 2.0 License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Hypothetical](https://img.shields.io/badge/Status-Hypothetical%20%2F%20Research-orange.svg)]()
[![Open Source](https://img.shields.io/badge/Open-Source-green.svg)]()

---

## ⚠️ Important Disclaimer

**This tool is entirely hypothetical and AI-generated. It is designed for research, education, and exploratory thinking only.**

- This is **not** clinical advice
- This is **not** regulatory guidance
- This is **not** an implementation specification or product
- All residents, names, data, workflows, confidence thresholds, and clinical scenarios are **fabricated and illustrative**
- All role descriptions, agent behaviours, and AN-ACC classifications are **approximate and for thinking purposes only**
- No part of this tool should be used to inform, guide, or justify any real clinical, operational, or regulatory decision

Always consult qualified clinicians, aged care specialists, and the [Aged Care Quality and Safety Commission](https://www.agedcarequality.gov.au/) before implementing any AI system in a care setting.

**Do your own research.**

---

## What This Is

The Agentic Aged Care Explorer is a single-file interactive HTML tool that models a hypothetical dual-layer agentic framework for residential aged care in Australia.

The central question it explores:

> *If AI agents could absorb the cognitive and administrative weight of a role — what would humans be freed to do instead?*

It is a thinking tool. A provocation. Not a prescription.

The framework models every major role in a residential aged care multidisciplinary team (MDT), splitting each into two layers:

- **AI agent layer** — handles cognitive, digital, and administrative tasks (drafting, triaging, scheduling, documenting, flagging, analysing)
- **Human layer** — physically acts, signs, decides, cares, and holds legal and clinical accountability

A **confidence gate** governs every handoff between the two layers. Humans can override at any point. Every decision is logged to an audit trail.

---

## What's Inside

The tool is a single self-contained HTML file (~242KB) with no server dependencies. It includes 14 interactive sections:

| Section | What it covers |
|---|---|
| **About** | Purpose, audience, the core idea, and open source licence |
| **Overview** | Framework summary, radar charts, automation potential by role |
| **Agent Pipeline** | Swimlane workflow diagram — 8 stages, 5 lanes, all agent touchpoints |
| **Role Map** | Dual-layer breakdown of every role — agent tasks vs human tasks |
| **Agent Registry** | Catalogue of all 22 named agents — domain, trigger, HITL rule, ACQS alignment |
| **Clinical Heatmap** | Task × role matrix showing who does what, filterable by criticality |
| **RN Deep Dive** | Detailed agentic workflow for the Registered Nurse role — shift start, Joe's fall case study, medication round, GP handoff, family communications |
| **Pre-Admission** | Multi-agent workflow from referral to admission + sample AI-generated assessment report |
| **Resident Deep Dive** | Joe Thornton — profile, risk flags, monthly trends, daily view, wellbeing, end-of-life planning, and all agent intersections |
| **Relationship Graph** | Force-directed network of all roles, agents, data flows, and handoff points |
| **Confidence Gate Simulator** | Interactive sliders — tune risk parameters, see where work routes |
| **Workload Analysis** | Agent vs human split by role, hours freed per shift, escalation rates |
| **Compliance** | All 8 ACQS Standards mapped to framework elements |
| **Glossary** | 30 plain-language definitions — agentic AI, clinical, regulatory, and framework terms |

---

## The Core Framework

### Dual-layer model

Every role has two layers. The agent handles the cognitive load. The human handles everything that requires physical presence, legal accountability, or irreplaceable human judgement.

```
Trigger / event
    ↓
AI Agent (enrichment → routing → specialist agents → validation → summary)
    ↓
Confidence Gate
    ↓ high confidence + low risk     ↓ low confidence or high risk
Agent acts autonomously          Human physically acts
Human notified                   Agent prepares brief + hands off
    ↓                                ↓
Audit trail logged           Audit trail logged
```

### The confidence gate

Every task passes through a confidence gate. Five parameters determine routing:

- Agent confidence score
- Clinical risk level
- Resident acuity
- Task urgency
- Regulatory sensitivity

The gate routes to one of three outcomes: autonomous agent action, human-in-the-loop review, or full physical handoff.

### Human-in-the-loop (HITL)

The HITL bridge is the architectural centre of the framework. It is not an optional layer — it is mandatory at every point where:

- A physical human must act (medication administration, wound care, personal care)
- A legal signature is required (care plans, medication charts, regulatory submissions)
- Clinical judgement is needed in novel or uncertain situations
- A family member needs to be contacted
- An end-of-life or consent decision arises

---

## The Case Study — Joe Thornton

Joe Thornton is the hypothetical resident who appears across three sections of the tool — Pre-Admission, RN Deep Dive, and Resident Deep Dive. He is the same person at different stages of his journey.

He is 84, has mixed dementia, dysphagia, osteoporosis, and is on Warfarin. He has had four falls in the past year. His son David is his primary contact and Medical Power of Attorney. His wife Margarete passed in 2018.

Joe is entirely fictional. He exists to make the framework concrete — to show how the agents, the HITL gates, the family comms workflow, and the AN-ACC monitoring all converge around a single human life.

---

## Regulatory Context

The framework is mapped to the Australian aged care regulatory environment:

- **Aged Care Act 1997** — primary legislation governing residential aged care
- **Aged Care Quality Standards (ACQS)** — all 8 standards addressed in the Compliance section
- **AN-ACC** — Australian National Aged Care Classification funding model
- **Aged Care Quality and Safety Commission (ACQSC)** — the independent regulator

All 22 agents in the registry are mapped to the ACQS standards they affect. The confidence gate design ensures human accountability is preserved at every regulatory touchpoint.

---

## Translating to Other Industries

The dual-layer model — agent handles cognitive load, human handles physical presence and legal responsibility — is not specific to aged care. The same pattern applies wherever:

- Cognitive and administrative burden is high
- Physical presence or specialist judgement is irreplaceable
- Regulatory accountability requires human sign-off
- Consistency across shift changes matters

Replace "RN" with "teacher", "carer" with "support worker", "ACQS" with your sector's regulatory framework. The architecture holds.

Sectors where this thinking directly applies: disability support, mental health services, community health, general practice, emergency services, construction site safety, legal case management, social work, education, and hospitality.

---

## Open Source

This tool is released under the **Apache License 2.0**.

You are free to:
- Use it for any purpose — personal, educational, commercial, research
- Modify it, adapt it, translate it to your sector
- Distribute it and build derivative works

You must:
- Include the Apache 2.0 licence notice with any redistribution

You cannot:
- Hold the author liable for any outcomes arising from use
- Use the author's name to endorse derivative works without permission

The full licence text is available at [apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0) and is embedded in the HTML file itself.

Attribution is welcome but not required. If this sparks something useful — in any sector, in any context — share it forward.

---

## Usage

This is a single self-contained HTML file. No build process, no server, no dependencies beyond two CDN-loaded libraries (Chart.js and D3.js).

**To use locally:**
```
1. Download aged_care_mdt_v4.html
2. Open in any modern browser
3. No installation required
```

**To host on GitHub Pages:**
```
1. Rename file to index.html
2. Create a public GitHub repository
3. Upload index.html
4. Go to Settings → Pages → Deploy from branch (main, root)
5. Live at yourusername.github.io/your-repo-name
```

---

## Credits

Built as a hypothetical thought experiment using Claude (Anthropic) to explore agentic AI modelling in a real-world care context. Designed to invoke deep thinking in both technical and non-technical audiences about how humans and AI agents can work together — not as a replacement model, but as a collaboration model.

---

*Not clinical advice. Not regulatory guidance. Not an implementation specification. Hypothetical only. Do your own research.*
