# Research Skill Templates

Reusable Claude Code skills distilled from "Levels of Using AI in Research" (AI day, 08/09/2026). Each one is set to `disable-model-invocation: true`, so Claude never triggers it on its own — it only runs when a user types the command. Since SKILL.md is an open standard, the same files also work as prompt templates in ChatGPT, Codex CLI, Gemini, and Copilot.

## Install (Claude Code)
Copy any skill folder into `~/.claude/skills/` (available in every project) or a project's `.claude/skills/` (that project only). If the destination skills folder didn't exist yet at session start, restart Claude Code once so it gets watched.

## Skills

| Command | What it does |
|---|---|
| `/grant-evaluator [funder]` | Strict funder-style critique of a proposal section — logical gaps, weak impact pathways, unconvincing methodology (default: Horizon Europe) |
| `/bias-omission-check` | Flags blind spots, inclusivity gaps, underrepresented stakeholders |
| `/grill-me-for-research [n]` | Skeptical senior PI interrogates the proposal one question at a time, then summarizes the weakest points |
| `/deconstruct-call [topic]` | Turns a funding call text into a compliance & KPI checklist |
| `/plain-language-polish` | Rewrites jargon for a diverse evaluation board without losing accuracy |
| `/consistency-check [style]` | Checks formatting and citation-style consistency across a proposal |
| `/fwo-admissibility-check` | FWO's own official eligibility rules — supervisor criteria, Junior/Senior, submission limits, budget, form completeness, formatting |
| `/fwo-reviewer [INTDIS]` | Simulates an FWO panel review scored against FWO's real scoring grid (Team / Originality / Feasibility / Interdisciplinarity) |
| `/llm-wiki [ingest\|query\|lint]` | Persistent markdown knowledge wiki instead of re-searching raw sources on every question |

## Attribution
Skill bodies are kept free of attribution text to avoid loading it into context on every invocation — credited here instead:
- **`/grant-evaluator`, `/bias-omission-check`, `/deconstruct-call`, `/plain-language-polish`** — adapted from prompts by Mads Lykke Berggreen (research adviser, VIA University College, Denmark; active in EARMA's AI community).
- **`/grill-me-for-research`** — adapted from Matt Pocock's `/grill-me` coding skill (74k+ GitHub stars).
- **`/consistency-check`, `/fwo-admissibility-check`, `/fwo-reviewer`, `/llm-wiki`** — no single-source attribution: either a general pattern from the slide deck (`/consistency-check`, `/llm-wiki`) or rebuilt from OBI's own FWO knowledge base rather than the original slide prompt (`/fwo-admissibility-check`, `/fwo-reviewer`).
