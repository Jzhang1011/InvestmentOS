InvestmentOS
A portable, model-agnostic investment thesis library for monitoring structural investment ideas.
Purpose
InvestmentOS separates three layers:
Knowledge — investment methodology, assumptions, indicators, patterns, and thesis files.
Analysis — manual analysis today; AI API or workflow automation later.
Publishing — approved decision briefs for WealthLanding or other channels.
The repository is designed so that the knowledge remains usable across ChatGPT, Gemini, Claude, local models, or future AI systems.
Current Scope
Version 1 includes the first active thesis:
JPY Structural Weakness
Repository Structure
```text
InvestmentOS/
├── README.md
├── framework/
│   ├── investment_methodology.md
│   └── analyst_instructions.md
├── templates/
│   ├── thesis_template.md
│   └── decision_brief_template.md
├── theses/
│   └── jpy/
│       ├── README.md
│       ├── thesis.md
│       ├── carry_trade.md
│       ├── monitoring_indicators.md
│       ├── boj_policy.md
│       ├── investment_opportunities.md
│       ├── pattern_recognition.md
│       └── assumption_map.md
├── outputs/
│   └── jpy/
│       └── README.md
└── docs/
    └── workflow.md
```
How to Use It Now
Open the relevant thesis folder.
Provide the framework files and thesis files to an AI model.
Ask the model to research developments since the prior review.
Require the decision brief format.
Review the output before making or publishing any investment conclusion.
Save approved briefs under `outputs/<thesis>/`.
Future WealthLanding Workflow
```text
GitHub InvestmentOS
        ↓
Scheduled backend job
        ↓
Current data and source retrieval
        ↓
AI API analysis
        ↓
Draft decision brief
        ↓
Human approval
        ↓
WealthLanding publication
```
Governance Principles
Price movement alone is not evidence.
Each conclusion must map to a thesis assumption.
Primary sources receive priority.
Public outputs require human review.
AI providers are replaceable; the knowledge base is permanent.
This repository is for research and education, not individualized financial advice.
Recommended Repository Setting
Keep the repository private while the methodology and private research are being developed. Publish only approved educational outputs through WealthLanding.
