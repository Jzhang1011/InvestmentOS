# InvestmentOS Workflow

## Current Manual Workflow

1. Update the relevant thesis files when your structural view changes.
2. Open the framework and thesis files in an AI-capable workspace.
3. Request a review covering a defined date range.
4. Require current source verification.
5. Generate a decision brief.
6. Verify facts, dates, officeholders, rates, and citations.
7. Save the approved brief in `outputs/<thesis>/`.
8. Publish an educational version to WealthLanding when appropriate.

## Suggested Prompt

> Use `framework/analyst_instructions.md`, `framework/investment_methodology.md`, and all files under `theses/jpy/`. Review developments since <DATE>. Use current primary and authoritative sources. Map each material fact to the relevant assumption. Produce `templates/decision_brief_template.md`. Do not treat price movement alone as evidence. Flag uncertain or conflicting facts.

## Future Automated Workflow

```text
Scheduled trigger
    ↓
Retrieve selected GitHub files
    ↓
Retrieve current primary-source evidence
    ↓
Call AI API with structured output
    ↓
Validate required fields
    ↓
Save draft brief
    ↓
Human approval
    ↓
Publish to WealthLanding
```

## Recommended Technical Components Later

- GitHub: canonical knowledge repository
- Serverless function or workflow engine: orchestration
- AI API: analysis
- Market/economic APIs: numerical data
- Database or GitHub outputs folder: history
- Email or dashboard: alerts
- Human approval: publication control

## Security

- Never store API keys in the repository.
- Use environment variables or a secret manager.
- Keep private investment research in a private repository.
- Expose only approved public content.
- Add rate limits before allowing public AI interaction.
