# Research Prompts

The same 9 skills from this folder, written out as plain copy-paste prompts instead of Claude Code SKILL.md files. Use these in any chat tool (ChatGPT, Gemini, Copilot, Claude.ai, etc.) that doesn't support the SKILL.md standard — paste the prompt, then paste or attach your proposal/text where indicated.

---

## Grant Evaluator

```
Act as a strict [funder — default Horizon Europe, e.g. FWO] grant evaluator. Read the following draft section of my proposal.

- Identify logical gaps, weak impact pathways, and unconvincing methodology claims.
- Give me 3 concrete, specific ways to make this argument sharper and more authentic.

[Paste or attach the draft proposal section here]
```

---

## Bias & Omission Check

```
Review this project concept text as a critical, independent reviewer.

- Highlight any invisible blind spots.
- Flag lack of inclusivity.
- Flag underrepresented stakeholder perspectives that a human panel might penalize.

Be specific — point to the sentence or section, not just the general theme.

[Paste or attach the project concept text here]
```

---

## Grill Me For Research

```
You are a skeptical senior PI reviewing a colleague's research proposal — not helping write it, interrogating it.

Ask one hard question at a time about the proposal pasted below. Focus on the core claim, why it's novel, what could make it fail, and whether the method actually tests the hypothesis.

Don't move on until I've given a real answer — push back if it's vague.

Stop after 8-10 questions, then summarize the 3 weakest points still unresolved.

[Paste or attach the proposal here]
```

---

## Deconstruct The Call

```
Act as a collaborative team of EU funding advisors. Deconstruct this call text for [insert topic] and list:

- The mandatory compliance hurdles.
- The core KPIs (Key Performance Indicators).
- The strategic alignment requirements we must address in the work package.

[Paste or attach the call text here]
```

---

## Plain-Language Polish

```
Take this heavily jargon-filled project summary and rewrite it to retain technical accuracy while improving readability and engagement for a diverse evaluation board.

Show the rewritten version, and note any term you simplified that I may want to double-check for precision.

[Paste or attach the project summary here]
```

---

## Consistency Check

```
Check this proposal for consistency:

- Fonts and heading styles.
- Table and figure numbering and captions.
- Section numbering.
- Every reference against [insert citation style, e.g. APA / Vancouver / IEEE] — flag any that don't match.

Offer to convert the whole reference list to a different target style if I ask.

[Paste or attach the proposal here]
```

---

## FWO Admissibility Check

```
Run FWO's official pre-submission eligibility & admissibility check for Fundamental Research Projects (Jr/Sr) on the proposal and applicant details below. A single FAIL in any section is enough to make the application inadmissible — report pass/fail per section with the article reference where given.

1. Applicant roles — supervisor-spokesperson must meet at least one of: ZAP/equivalent + PhD + ≥50% FTE at a Flemish main host institution; OR ZAP ≥10% + FWO fellowship or qualifying appointment totalling ≥70% FTE; OR ZAP ≥5% + Flemish Academic Hospital clinical head role; OR FWO research director; OR ERC grantee at a Flemish host; OR Odysseus II grantee at a Flemish university. If none apply: FAIL (art. 10). Co-supervisors must be at postdoctoral level or equivalent; non-Flemish co-supervisor capped at 10% of total budget.

2. Junior/Senior classification — reference date 1 April of the call year. PhD ≤12 years before that date = Junior, otherwise Senior. Career-age extensions (≥3 months each) apply for maternity/parental/sickness leave, mandatory military/civic service, or other documented interruptions — must be declared in the e-portal.

3. Submission limits — max 1 application per role this call (incl. WEAVE); max 2 ongoing + newly requested projects simultaneously as (co-)supervisor (reference date 1 January after the call); a co-supervisor whose institution isn't requesting budget doesn't count.

4. Host institution eligibility — main host institutions: the 5 Flemish universities (UHasselt, KU Leuven, UAntwerpen, UGent, VUB), Evangelic Protestant Faculty Leuven / Faculty for Protestant Theology Brussels, Maritime Academy, Vlerick Business School, Antwerp Management School, Institute for Tropical Medicine, or one of 8 Flemish Schools of Arts. Non-main host institutions (co-PI only, budget capped): recognised Flemish/federal research institutes, or non-Flemish institutes (max 10% of total budget).

5. Budget compliance — min €50,000/year for the whole project; max €145,000/year per institution (or combined, if one person represents multiple institutions); equipment >€20,000/unit capped at €150,000 for the whole project; non-Flemish institution share capped at 10%; project duration min 2 years, standard 4 years. Use the applicant's own host institution's staff cost rates to check budget lines — these vary by institution.

6. VIB cap (if applicable) — check whether the chosen panel already has >50% of its budget on VIB-only projects, and whether there's ≥1 non-VIB (co-)supervisor (if yes, the cap doesn't apply).

7. Retired professors (emeriti) — if retiring during submission year or project period, confirm a ZAP co-promotor at the same main host institution is included, with a succession plan noted.

8. Dual institutional representation — if one person represents multiple institutions, confirm total budget across all of them is ≤€145,000/year.

9. Application form completeness — personalia (ORCID, addresses, degrees, positions), Junior/Senior track selected, host institutions & supervisors tab, research statement, CV ≤4 pages, 5 main publications/achievements, project description (Word template, ≤10 pages — violations make it inadmissible), rationale/state-of-the-art, scientific objectives, methodology/work plan, references, other funding disclosure (mandatory), contentwise/conceptual contribution, ethics checklist, Research Security tab, Data Management Plan, consent forms if applicable, submitted via host institution.

10. Formal format check — ≤10 A4 pages incl. references/figures/tables; Calibri 11 (Carlito 11 for LaTeX); line spacing 1; 2.5cm margins all sides; no external links/hyperlinks; section titles retained.

Report using this template:

ADMISSIBILITY CHECK — [Applicant name] — [Call year]
ELIGIBILITY: PASS / FAIL (supervisor-spokesperson / Junior-Senior / submission limit / host institution)
BUDGET: PASS / FAIL / REVIEW NEEDED (per institution vs €145k, equipment vs €150k, issues)
FORM COMPLETENESS: complete / missing: [list]
FORMAT: OK / issues: [list]
OVERALL: ADMISSIBLE / INADMISSIBLE / ISSUES TO RESOLVE BEFORE SUBMISSION

This is a pre-submission sanity check, not an official FWO ruling — the binding regulations are in Dutch.

[Paste or attach the proposal and applicant details here]
```

---

## FWO Reviewer

```
Simulate an FWO expert-panel reviewer for the Fundamental Research Projects programme (Jr/Sr) on the proposal below. Panel type: [regular panel, or write "INTDIS" for the Specific Interdisciplinary Panel].

Scoring scale: 0 Unacceptable · 1 Weak · 2 Fair · 3 Reasonable · 4 Good · 5 Very Good · 6 Excellent · 7 Outstanding.

Weighting: Criterion 1 (Team) 25%. Criterion 2 (Project = 2a+2b) 75% for regular panels, 55% for INTDIS. Criterion 3 (Interdisciplinarity) 20%, INTDIS panels only. Budget is not a scoring criterion.

Criterion 1 — Research Team (25%): scientific capacity, track record, and collaboration of the supervisor-spokesperson, (co-)supervisors, and research team(s) — competences, infrastructure, quality/impact of output, collaboration.

Criterion 2a — Scientific quality, relevance & originality: does the project meaningfully advance the international state-of-the-art, is it original, will it generate new knowledge?

Criterion 2b — Research approach & feasibility: is the approach appropriate and feasible in 4 years, is staffing adequate, are resources well estimated? A score of 4+ requires explicit transparency/reproducibility measures.

Criterion 3 — Interdisciplinarity (INTDIS only, min. score 4 required for funding): more than one sufficiently distinct discipline, at the same coordinated level, each essential to the outcome, with state-of-the-art advanced in all of them or a shared area.

Mandatory checks — flag explicitly if triggered:
- PI involvement in workpackages: if the PI's own role is absent or vague in the WP descriptions (vs. just the PhD student/co-investigators), flag as a Criterion 1 weakness.
- Ethics with minors: if the research involves children or other vulnerable groups, verify both parental/guardian informed consent AND age-appropriate assent from the children themselves; flag if only guardian consent is mentioned.
- Criterion 2b ≥4 threshold: confirm explicit transparency/reproducibility measures are present; flag as required if absent.
- Budget ↔ work plan cross-check: for each major budget line, verify a matching activity/work package/Gantt milestone exists; flag any that don't.

Output format — follow exactly:

### Criterion 1 — Research Team (weight: 25%)
Score: [0–7] — [band label]
Strengths: [2–4 sentences, reviewer voice, citing specific proposal text]
Weaknesses: [2–4 sentences, or "No significant weaknesses identified."]
General remarks and suggestions for improvement regarding the project: [1–3 actionable sentences]

### Criterion 2a — Scientific quality, relevance & originality
Score: [0–7] — [band label]
Strengths: [...]
Weaknesses: [...]

### Criterion 2b — Research approach & feasibility
Score: [0–7] — [band label]
Strengths: [...]
Weaknesses: [...]
General remarks and suggestions for improvement regarding the project: [...]
Conclusion: [2–4 sentences on overall strength and main condition(s) for funding]

### Criterion 3 — Interdisciplinarity (INTDIS panels only — omit otherwise)
Score: [0–7] — [band label]
Strengths: [...]
Weaknesses: [...]

### Appropriateness of the requested budget (not scored)
1. Overall reasonableness relative to planned activities.
2. Budget ↔ work plan cross-check results.

### Weighted total and recommendation
Criterion 1: [score] × 0.25 = [weighted]
Criterion 2 (2a+2b combined): [score] × 0.75 (or 0.55 for INTDIS) = [weighted]
Criterion 3 (INTDIS only): [score] × 0.20 = [weighted]
Total: [sum out of 7]
Recommendation: Fundable / Borderline / Not fundable — [one-sentence justification]

### Improvement suggestions
Numbered list, advisor voice ("We recommend…"), one item per weakness above: what to fix, where in the document, why it matters to the panel.

### Caveat (always include, verbatim)
"This is a simulated review based on the FWO scoring rubric. It does not represent an actual FWO evaluation and cannot predict panel ranking or funding outcomes."

[Paste or attach the full proposal here]
```

---

## LLM Wiki

```
Help me maintain a persistent markdown knowledge wiki instead of re-reading raw sources from scratch every time.

Structure:
- raw/ — untouched source documents, never edited.
- wiki/ — the pages you maintain (entity pages, topic summaries, an index).
- A schema file (e.g. CLAUDE.md at the wiki's root) telling you how to file, cross-reference, and answer from it.

If this structure doesn't exist yet, ask me where the wiki should live and create raw/, wiki/, wiki/index.md, and a schema file before proceeding.

Pick one mode:
- Ingest: read the new source I give you, then update the relevant wiki pages (entity pages, topic summaries, the index). Flag anything that contradicts what's already there.
- Query: check wiki/index.md first, then the pages it points to, and answer from what the wiki already knows. Don't start from the raw sources unless the wiki is silent on the question.
- Lint: health-check the wiki — orphan pages, stale claims, missing cross-references. Report findings; don't fix silently.

Mode: [ingest / query / lint]
[Name the source, or ask your question, here]
```
