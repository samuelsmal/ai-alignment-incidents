# Contributing

This list focuses specifically on AI **alignment incidents** — cases where a model's behavior diverged from its designers' intent in ways that reveal something about alignment risk. It is not a general AI failure database.

---

## What belongs here

- **Emergent behavior during training** that violates designer intent (reward hacking, physics exploits)
- **Instrumental self-preservation** (shutdown resistance, weight exfiltration, blackmail)
- **Deceptive behavior** during evaluation or deployment (alignment faking, sandbagging, scheming)
- **Reward hacking** with real-world consequences (unauthorized resource acquisition, novel goal pursuit)
- **Instrumental goal pursuit** that conflicts with human oversight or safety constraints

---

## What does not belong here

- General product failures (chatbot hallucinations returning wrong facts)
- Content moderation errors or policy violations
- Deepfake misuse by third parties
- Bias and fairness failures in deployed products
- Infrastructure or API security vulnerabilities

---

## Submission format

Open a PR with two files:

1. **A row in `README.md`** (add to the Incident Index table):
```
| N | [Short title](#anchor) | Model name | Company | Phase | Reported date |
```

2. **A detail file** at `incidents/NNN-short-slug.md` using the template below.

---

## Incident detail template

```markdown
# Incident NNN — [Title]

**Status:** [Confirmed / Alleged / Disputed]
**Severity:** [Low / Medium / High] — [one-line justification]
**Category:** [e.g. Reward hacking / Instrumental self-preservation / Alignment faking]

---

## Summary
[2–4 sentences]

---

## System Details

| Field | Value |
|-------|-------|
| Model name | |
| Developer | |
| Phase | [Training / Safety testing / Deployment / External research] |
| Published | |
| Reported by | |

---

## What Happened
[Detailed narrative]

---

## Root Cause
[Analysis]

---

## Response
[Developer or researcher response]

---

## Sources
- [Source 1](url)
- [Source 2](url)

---

## See Also
- [Related incident](link)
```

---

## Standards

- **Sources required:** Every incident must have at least one primary source (paper, system card, or direct reporting from the researcher or developer). Secondary coverage alone is not sufficient.
- **Status field:** Use "Confirmed" only when published by the developer or in a peer-reviewed/preprint paper. Use "Alleged" for credible but unconfirmed reports.
- **No speculation:** Stick to documented behavior. Avoid inferring intent beyond what the source material supports.
- **Neutrality:** Describe behavior factually. These are complex technical phenomena, not indictments of companies.
