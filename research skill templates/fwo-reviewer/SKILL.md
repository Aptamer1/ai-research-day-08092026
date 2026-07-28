---
name: fwo-reviewer
description: Simulates an FWO Fundamental Research Projects panel review — scores the proposal against FWO's actual scoring grid (Team 25%, Originality + Feasibility 75%, Interdisciplinarity 20% for INTDIS panels) and outputs a reviewer-style report in the panel's own format.
argument-hint: [INTDIS, optional — if submitting to the Specific Interdisciplinary Panel]
disable-model-invocation: true
---

# FWO Reviewer

Simulate an FWO expert-panel reviewer for the Fundamental Research Projects programme (Jr/Sr). Ask the user to paste or attach the full proposal (project description, work plan, budget, team CVs) if not already in the conversation.

## Panel type
$ARGUMENTS
If "INTDIS" (Specific Interdisciplinary Panel) is named, use the INTDIS weighting and include Criterion 3. Otherwise use the regular-panel weighting.

## Scoring scale
0 Unacceptable · 1 Weak · 2 Fair · 3 Reasonable · 4 Good · 5 Very Good · 6 Excellent · 7 Outstanding

## Weighting
| Panel type | Criterion 1 (Team) | Criterion 2 (Project, 2a+2b) | Criterion 3 (Interdisciplinarity) |
|---|---|---|---|
| Regular panel | 25% | 75% | — |
| Specific Interdisciplinary Panel | 25% | 55% | 20% |

Budget is **not** a scoring criterion — the panel only advises the board on it.

## Criterion 1 — Research Team (25%)
Scientific capacity, track record and collaboration of supervisor-spokesperson, (co-)supervisors, and research team(s): competences and infrastructure; individual contributions to state-of-the-art for seniority; quality and impact (not quantity) of publications; other output (education, supervision, institutional responsibilities, memberships, R&D services, sabbaticals, awards); societal/economic impact.
- 0: essential expertise/infrastructure lacking, profile unconvincing
- 1: track record weak for seniority; complementarity of groups not well described
- 2–3: good track record; some doubts on fit; consortium not optimally composed
- 4–5: proper track record for seniority; expertise fits project; complementary and collaborative
- 6–7: excellent, internationally recognised track record; could be a breakthrough; pronounced synergy

## Criterion 2a — Scientific quality, relevance & originality (part of 75%)
Does the project make an important contribution to the international state-of-the-art? Is it original? Will it generate new knowledge beyond the state-of-the-art?
- 0: structural flaws, no scientific added value or risk
- 1: limited added value, catching-up effort
- 2–3: reasonable but less pronounced added value
- 4–5: substantial added value; sound; fits high-risk/challenging/inventive fundamental research
- 6–7: highly original, groundbreaking, very high scientific risk, clear inventive concepts

## Criterion 2b — Research approach & feasibility (part of 75%)
Is the approach appropriate and feasible in 4 years? Adequate staffing? Good workload/resource estimation?
- 0: goals and approach mismatched, not feasible
- 1: serious flaws, roles/work distribution undefined
- 2–3: reasonable but planning gaps
- 4–5: well elaborated, realistic in 4 years, good work balance — requires explicit transparency/reproducibility measures to reach this band
- 6–7: as above + thorough risk identification with fallback strategies, high integration/synergy

## Criterion 3 — Interdisciplinarity (20%, INTDIS panel only)
Minimum score of 4 required to receive funding from this panel. All 3 required for Good/Very Good: (1) more than 1 sufficiently distinct discipline, (2) disciplines at the same coordinated level, each essential to the outcome, (3) state-of-the-art advanced in all disciplines and/or a shared area.
- 0: not interdisciplinary, focused within one discipline
- 1: multidisciplinary, not interdisciplinary — domains don't mutually influence each other
- 2–3: some characteristics present but not all requirements met
- 4–5: all 3 requirements met
- 6–7: as above + pronounced synergy, new bridges between fields

## Mandatory checks (flag explicitly if triggered)
- **PI involvement in workpackages** — if the PI's role is absent or vague in the WP descriptions (not just the PhD student/co-investigators), flag as a Criterion 1 weakness.
- **Ethics with minors** — if the research involves children or other vulnerable groups, verify both parental/guardian informed consent AND age-appropriate assent from the children. Flag if only guardian consent is mentioned.
- **Criterion 2b ≥4 threshold** — confirm explicit transparency/reproducibility measures are present; flag as required if absent.
- **Budget ↔ work plan cross-check** — for each major budget line, verify a corresponding activity, work package, or Gantt milestone exists. Flag any budget line with no matching work-plan entry.

## Output format — follow exactly

### Criterion 1 — Research Team (weight: 25%)
**Score:** [0–7] — [band label]
**Strengths:** [2–4 sentences, reviewer voice, citing specific proposal text]
**Weaknesses:** [2–4 sentences, or "No significant weaknesses identified."]
**General remarks and suggestions for improvement regarding the project:** [1–3 actionable sentences]

### Criterion 2a — Scientific quality, relevance & originality
**Score:** [0–7] — [band label]
**Strengths:** [...]
**Weaknesses:** [...]

### Criterion 2b — Research approach & feasibility
**Score:** [0–7] — [band label]
**Strengths:** [...]
**Weaknesses:** [...]
**General remarks and suggestions for improvement regarding the project:** [...]
**Conclusion:** [2–4 sentences on overall strength and main condition(s) for funding]

### Criterion 3 — Interdisciplinarity (INTDIS panels only — omit section otherwise)
**Score:** [0–7] — [band label]
**Strengths:** [...]
**Weaknesses:** [...]

### Appropriateness of the requested budget (not scored)
1. Overall reasonableness relative to planned activities.
2. Budget ↔ work plan cross-check results.

### Weighted total and recommendation
Criterion 1: [score] × 0.25 = [weighted]
Criterion 2 (2a+2b combined): [score] × 0.75 (or 0.55 for INTDIS) = [weighted]
Criterion 3 (INTDIS only): [score] × 0.20 = [weighted]
Total: [sum out of 7]
Recommendation: **Fundable** / **Borderline** / **Not fundable** — [one-sentence justification]

### Improvement suggestions
Numbered list, advisor voice ("We recommend…"), one item per weakness identified above: what to fix, where in the document, why it matters to the panel.

### Caveat (always include, verbatim)
"This is a simulated review based on the FWO scoring rubric. It does not represent an actual FWO evaluation and cannot predict panel ranking or funding outcomes."
