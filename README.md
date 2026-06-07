# EI PSM Framework Audit Tool
### Process Safety Management — All 20 Elements | AI-Assisted Scoring | Professional Report Generation

> A fully browser-based, AI-powered process safety management audit tool covering all 20 elements of the **Energy Institute (EI) High Level Framework for Process Safety Management**. Designed for oil and gas facilities, refineries, chemical plants, and any major accident hazard (MAH) site. Deployable from GitHub Pages with zero server infrastructure required.

---

## Live Deployment

Deploy to GitHub Pages in 3 steps:
1. Fork this repository or upload `index.html` and `README.md` to a new repository root
2. Go to **Settings → Pages → Deploy from branch → main / root → Save**
3. Your tool is live at `https://[username].github.io/[repo-name]/`

No build process. No Node.js. No server. Single HTML file — it just works.

---

## What This Tool Does

This application provides a comprehensive digital audit platform for assessing an organisation's compliance with the EI PSM Framework across all 20 process safety management elements. It supports:

- **Structured audit questioning** with 4-level scoring (Major Deficiency to Exceeds Expectations)
- **Two audit modes**: Light (quick gap assessment) and Detailed (full EI expectation-based audit)
- **AI-assisted scoring** — describe your findings and the AI suggests an appropriate score with justification
- **AI professional note rewriting** — converts raw field notes into formal audit report language
- **Automated report generation** — produces a complete professional audit report with AI narrative
- **Progress tracking** across all 20 elements with real-time compliance dashboard
- **Data persistence** via browser localStorage — your audit survives browser restarts
- **Export/import** — save your audit data as JSON and share with colleagues

---

## Question Coverage

| Mode | Questions | Description |
|------|-----------|-------------|
| Light Mode | 89 questions | 4-5 targeted questions per element for rapid gap assessment |
| Detailed Mode | 445 questions | Comprehensive question bank covering every EI PSM Framework expectation |

### Detailed Mode Question Bank

The Detailed Mode is built directly from the EI PSM Framework guidance documents (Elements 1-20), structured across three audit phases per element:

- **Phase 1 — Set-up and Preparation**: Roles, competencies, standards, planning, and gap analysis
- **Phase 2 — Operations and Implementation**: Execution, controls, communication, and compliance
- **Phase 3 — Monitor, Review, and Intervene**: Performance measurement, trend analysis, and annual review

---

## All 20 PSM Elements Covered

### Process Safety Leadership

| # | Element | Detailed Questions |
|---|---------|-------------------|
| 1 | Leadership, Commitment and Responsibility | 28 |
| 2 | Identification and Compliance with Legislation and Industry Standards | 21 |
| 3 | Employee Selection, Placement and Competency, and Health Assurance | 26 |
| 4 | Workforce Involvement | 18 |
| 5 | Communication with Stakeholders | 18 |

### Risk Identification and Assessment

| # | Element | Detailed Questions |
|---|---------|-------------------|
| 6 | Hazard Identification and Risk Assessment | 27 |
| 7 | Documentation, Records and Knowledge Management | 19 |

### Risk Management

| # | Element | Detailed Questions |
|---|---------|-------------------|
| 8 | Operating Manuals and Procedures | 18 |
| 9 | Process and Operational Status Monitoring and Handover | 20 |
| 10 | Management of Operational Interfaces | 16 |
| 11 | Standards and Practices | 23 |
| 12 | Management of Change and Project Management | 28 |
| 13 | Operational Readiness and Process Start-up | 23 |
| 14 | Emergency Preparedness | 22 |
| 15 | Inspection and Maintenance | 22 |
| 16 | Management of Safety Critical Devices | 23 |
| 17 | Work Control, Permit to Work and Task Risk Management | 23 |
| 18 | Contractor and Supplier Selection and Management | 20 |

### Review and Improvement

| # | Element | Detailed Questions |
|---|---------|-------------------|
| 19 | Incident Reporting and Investigation | 25 |
| 20 | Audit, Assurance, Management Review and Intervention | 25 |

---

## Scoring System

Every question uses a 4-level scoring scale aligned with the EI PSM Framework:

| Score | Label | Description |
|-------|-------|-------------|
| N/A | Not Applicable | Question does not apply to this operation |
| 1 | Major Deficiency | Arrangement not in place or completely inadequate |
| 2 | Minor Deficiency | Partially in place or significant gaps exist |
| 3 | Meets Expectations | Fully in place and functioning as intended |
| 4 | Exceeds Expectations | Exemplary — beyond EI PSM Framework requirements |

### 3-Column Scoring Guide

Every question in Detailed Mode includes a full 3-column scoring reference table (click "Scoring Guide & Evidence" on any question):

- **Column 1 — SCORE**: Score level and label (e.g. "Score 2 — Minor Deficiency")
- **Column 2 — SCORING CRITERIA**: Specific description of what the auditor should observe to justify that score
- **Column 3 — EVIDENCE TO EXAMINE**: 3-4 specific items to check, documents to request, or interviews to conduct

---

## AI Features

### Setting Up Your API Key

1. Open Settings (top right of the header)
2. Select your AI provider:
   - **OpenAI GPT-4o-mini** (Recommended — best browser support): Get your key at platform.openai.com/api-keys
   - **Anthropic Claude Haiku**: Get your key at console.anthropic.com
3. Paste your API key and click Save

Your API key is stored only in your browser's localStorage. It is never sent to any server other than the AI provider's API directly.

### AI Suggest Score

For any question, enter your audit findings in the notes field and click "AI Suggest Score". The AI will:
- Analyse your evidence against the 4-level scoring criteria
- Recommend the most appropriate score (1-4 or N/A)
- Provide a concise justification
- Identify key gaps in the evidence
- Suggest a specific corrective action

You can Accept the suggestion or override it with your own judgment.

### Rewrite Notes

Click "Rewrite Notes" to convert your raw field notes into formal professional audit report language. The AI:
- Preserves all factual content and observations
- Converts informal language to formal third-person audit style
- Structures the text clearly: findings first, then evidence basis

### AI Audit Report

After completing your audit, click "AI Report" on the Report page. The AI generates a complete professional audit report (20-40 seconds) containing:

1. **Executive Summary** — Overall assessment, key deficiency themes, key strengths, and immediate priorities
2. **Scope of the Audit** — Facility, methodology, elements covered, and audit mode
3. **Findings** — Narrative synthesis by PSM focus area
4. **Recommendations and Corrective Actions** — Prioritised by score level
5. **Closeout** — Summary table, sign-off blocks, next audit date recommendation

A Basic Report (no API key needed) generates the same structure as a formatted findings table.

---

## Using the Application

### Settings

Before starting your audit, open Settings and enter:
- **Facility / Plant Name** — the site or facility being audited
- **Lead Auditor** — your name
- **Audit Date** — date of the audit
- **Audit Type** — Annual Internal Audit, Third-Party Audit, Regulatory Audit, etc.
- **AI Provider and API Key** — for AI-assisted scoring and report generation

### Mode Toggle

The header shows two mode buttons:
- **Light (89 Q)** — Quick gap assessment with 4-5 questions per element
- **Detailed (445 Q)** — Full EI expectation-based audit with phase-structured questioning

Switching modes preserves all your scores and notes for each mode independently.

### Completing an Audit

1. Enter facility details in Settings
2. Select a mode (Light or Detailed)
3. Navigate to each element using the sidebar
4. Score each question by clicking the score buttons (N/A, 1, 2, 3, 4)
5. Enter findings in the notes field — be specific about what you observed, documents reviewed, and personnel interviewed
6. Use AI Suggest to get a score recommendation based on your notes
7. Generate a report when ready

### Dashboard

The Dashboard shows:
- **Overall Compliance %** — (average score minus 1) divided by 3 times 100
- **Score breakdown** — Count of Major Deficiencies, Minor Deficiencies, Meets, and Exceeds
- **Element grid** — All 20 elements with individual compliance scores
- **Rating** — Poor (<30%) | Fair (30-50%) | Adequate (50-70%) | Good (70-85%) | Excellent (>85%)

### Saving and Exporting

- **Auto-save**: All scores and notes automatically save to browser localStorage
- **Export**: Downloads your complete audit data as a JSON file for backup or sharing
- **Import**: Restores a previously exported audit session
- **Print**: Prints the current report to PDF via the browser print dialog

---

## Audit Report Structure

Both Basic and AI reports include:

**1. Executive Summary**
High-level assessment of overall PSM compliance, key themes in deficiencies, notable strengths, and top priority actions.

**2. Scope of the Audit**
Facility name, audit date, lead auditor, audit type, framework reference, and elements covered.

**3. Findings**
Narrative synthesis by PSM focus area calling out specific element performance, distinguishing major from minor deficiencies.

**4. Recommendations and Corrective Actions**
Prioritised corrective actions:
- Immediate / 30-day: Score 1 (Major Deficiency) items
- 90-day: Score 2 (Minor Deficiency) items
- Continuous improvement: Score 3-4 items with enhancement potential

**5. Closeout**
Summary table of scores, sign-off blocks for lead auditor and site representative, and next audit date recommendation.

---

## Data Privacy

- All audit data is stored locally in your browser (localStorage)
- No data is sent to any server except the AI provider's API (only when you use AI features)
- Only the text you type in notes fields is sent to the AI provider
- Your API key is stored in localStorage — clear it via Settings if sharing a device
- Use "Clear All Data" in Settings to permanently delete all audit data from the browser

---

## Technical Details

| Feature | Detail |
|---------|--------|
| Technology | Pure HTML/CSS/JavaScript — no frameworks, no build tools |
| File size | ~1.4 MB (single HTML file) |
| Dependencies | None — fully self-contained |
| AI (scoring) | OpenAI GPT-4o-mini or Anthropic Claude Haiku |
| AI (reports) | OpenAI GPT-4o-mini or Anthropic Claude Haiku |
| Data storage | Browser localStorage |
| PDF export | Browser Print API |
| Compatibility | Any modern browser (Chrome, Edge, Firefox, Safari) |
| Deployment | GitHub Pages, any static file host, or open locally |

---

## Question Data Structure

To add or update questions, modify the ELEMENTS JavaScript data in index.html. Each element follows this schema:

```javascript
{
  id: 1,                    // Element number (1-20)
  title: "...",             // Element title
  focus: "...",             // Focus area label
  icon: "...",              // Display emoji icon
  overview: "...",          // Element overview text
  questions: [...],         // Light mode questions (4-5 per element)
  dquestions: [...]         // Detailed mode questions (10-28 per element)
}
```

Each question:

```javascript
{
  id: "E1D01",             // Unique question ID
  exp: "1.1",              // EI PSM expectation reference
  text: "...",             // The audit question text
  guidance: "...",         // Brief auditor guidance
  c1: "...", e1: [...],    // Score 1 criteria + 3-4 evidence bullet points
  c2: "...", e2: [...],    // Score 2 criteria + 3-4 evidence bullet points
  c3: "...", e3: [...],    // Score 3 criteria + 3-4 evidence bullet points
  c4: "...", e4: [...]     // Score 4 criteria + 3-4 evidence bullet points
}
```

---

## Source Reference

Energy Institute. *High Level Framework for Process Safety Management*. London: Energy Institute, 2010.

Energy Institute. *Guidance on Meeting Expectations of EI Process Safety Management Framework*, Elements 1-20 (1st edition). London: Energy Institute, 2013.

The question bank in Detailed Mode is derived directly from the EI PSM Framework guidance documents, with questions structured around the formal expectations defined in each element's guidance publication.

---

## License

MIT License — free to use, modify, and deploy.

This tool is provided for general information and educational purposes. While it is based on the EI PSM Framework, it does not constitute formal regulatory compliance advice. Always consult applicable legislation and industry standards for your specific jurisdiction and operations.

---

*Built for the oil and gas industry. Powered by the EI PSM Framework.*
