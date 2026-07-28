---
name: fwo-admissibility-check
description: Runs FWO's own official pre-submission eligibility & admissibility check for Fundamental Research Projects (Jr/Sr) — supervisor-spokesperson criteria, Junior/Senior classification, submission limits, host institution eligibility, budget compliance, form completeness, and formatting. Funder-official rules, not tied to any one institution.
disable-model-invocation: true
---

# FWO Admissibility Check

A single FAIL in any section below is enough to make the application inadmissible. Ask the user to paste or attach the draft proposal and applicant details (name, current positions with FTE%, PhD date, institution affiliations) if not already in the conversation, then work through each section and report pass/fail with the article reference where given.

## 1. Applicant roles

**Supervisor-spokesperson (mandatory, 1 per project)** — must meet at least one:
- ZAP or equivalent appointment + PhD + ≥50% FTE at a Flemish main host institution
- ZAP ≥10% at main host institution + FWO research fellowship OR appointment at main host / Flemish academic hospital / hospital with academic character / recognised Flemish or federal research institution / SOC / Flemish School of Arts academic programme; total ≥70% FTE
- ZAP ≥5% at main host institution + appointment at a Flemish Academic Hospital as clinical head / assistant clinical head / equivalent
- FWO research director
- ERC grantee at a Flemish main host institution
- Odysseus II grantee with a Flemish university as main host

→ If none apply: **FAIL** (regulations art. 10)

**Supervisor (optional, ≤1 per partner main host institution)** — same requirements as above; mandatory for the entire project duration.

**Co-supervisors (optional)** — must be at postdoctoral level or equivalent, remunerated appointment at main host institution / Flemish School of Arts / recognised Flemish research institute / recognised federal scientific institute. Non-Flemish co-supervisor allowed, budget capped at 10% of total project budget.

## 2. Junior / Senior classification
Reference date: 1 April of the call year.
- PhD from ≤12 years before the reference date → **Junior**
- PhD >12 years before the reference date → **Senior**

Eligible career-age extensions (art. 10 §5), each reduces effective career age: maternity leave ≥3 months, parental leave ≥3 months, sickness leave ≥3 months, mandatory military/civic service ≥3 months, other documented career interruptions. All breaks must be declared in the e-portal.

## 3. Submission limits
- Max 1 application per role (supervisor-spokesperson, supervisor, or co-supervisor) in this call, including WEAVE projects
- Max 2 ongoing + newly requested fundamental research projects simultaneously as (co-)supervisor (reference date 1 January of the year after the call)
- Exception: a co-supervisor whose institution is not requesting budget does not count toward the limit

## 4. Host institution eligibility

**Main host institutions** (can hold primary/partner PI role): the 5 Flemish universities (UHasselt, KU Leuven, UAntwerpen, UGent, VUB), Evangelic Protestant Faculty Leuven / Faculty for Protestant Theology Brussels, Maritime Academy, Vlerick Business School, Antwerp Management School, Institute for Tropical Medicine, or one of 8 Flemish Schools of Arts.

**Non-main host institutions** (co-PI only, budget cap applies): recognised Flemish research institute, recognised federal scientific institute, or non-Flemish institute (max 10% of total budget).

## 5. Budget compliance
| Rule | Limit |
|---|---|
| Staff & consumables — minimum, entire project | Min €50,000/year |
| Staff & consumables — per institution | Max €145,000/year |
| One applicant representing multiple institutions | Max €145,000/year for ALL those institutions combined |
| Equipment (>€20,000/unit) | Max €150,000 for entire project |
| Non-Flemish institution share | Max 10% of total budget |
| Project duration | Min 2 years, standard 4 years |

Check the applicant's own host institution for its indicative staff cost rates — these vary by institution and aren't set by FWO itself. (UHasselt applicants: use `/obi-admissibility-check` for UHasselt's own rates and internal tracking fields.)

## 6. VIB cap (if applicable)
If any applicant is affiliated with VIB (group leader or VIB PI): check whether the chosen expert panel already has >50% of its budget going to VIB-only projects, and whether there's at least 1 non-VIB (co-)supervisor in the project (if yes, the cap doesn't apply).

## 7. Retired professors (emeriti)
If any applicant is retiring in the year of submission or during the project period: confirm a ZAP co-promotor at the same main host institution is in the application, noted with a succession plan.

## 8. Dual institutional representation
If one person represents multiple institutions: confirm total budget requested across all their institutions is ≤€145,000/year. Advise separating applicants across institutions if this maximizes budget.

## 9. Application form completeness
Personalia complete (ORCID, addresses, degrees, positions); Junior or Senior track selected; Host institutions & Supervisors tab complete; Research Statement; short CV ≤4 pages; 5 main publications/achievements; project description (Word template, ≤10 pages, correct format — violations make it inadmissible); rationale/state-of-the-art; scientific objectives; methodology/work plan; references; other funding disclosure (mandatory — failure risks exclusion next round); contentwise/conceptual contribution; ethics checklist; Research Security tab; Data Management Plan; consent forms for non-Flemish non-main host institutions if applicable; submitted via host institution (researcher submits to HI first, HI submits to FWO).

## 10. Formal format check (Word template)
≤10 A4 pages including references, figures, tables; font Calibri 11 (Carlito 11 for LaTeX); line spacing 1; margins 2.5cm all sides; no external links or hyperlinks; section titles retained.

## Output
Use this template:

```
ADMISSIBILITY CHECK — [Applicant name] — [Call year]

ELIGIBILITY: PASS / FAIL
  Supervisor-spokesperson: [criteria met]
  Junior/Senior: [track] (PhD: [year]; extensions: [list])
  Submission limit: [OK / issue]
  Host institution: [OK / issue]

BUDGET: PASS / FAIL / REVIEW NEEDED
  Per institution: €[x]/year (limit €145k)
  Equipment: €[x] (limit €150k)
  Issues: [none / list]

FORM COMPLETENESS: [complete / missing: list]
FORMAT: [OK / issues: list]

OVERALL: ADMISSIBLE / INADMISSIBLE / ISSUES TO RESOLVE BEFORE SUBMISSION
```

The official regulations are binding in Dutch; English is guidance only. This is a pre-submission sanity check, not an official FWO ruling.
