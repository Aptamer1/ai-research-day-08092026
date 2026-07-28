---
name: llm-wiki
description: Maintains a persistent markdown knowledge wiki instead of re-reading raw sources from scratch each time — ingest new sources into growing wiki pages, answer questions from what the wiki already knows, or lint the wiki for staleness. Use for a research topic, funder, or project you return to repeatedly.
argument-hint: [ingest|query|lint] [source path or question]
disable-model-invocation: true
---

# LLM Wiki

A persistent-memory pattern: sources are read once, then compiled into a growing markdown wiki instead of being re-searched from scratch on every question.

## Structure
- `raw/` — untouched source documents, never edited.
- `wiki/` — the pages you maintain (entity pages, topic summaries, an index).
- A schema file (e.g. `CLAUDE.md` at the wiki's root) telling you how to file, cross-reference, and answer from it.

If this structure doesn't exist yet in the current directory, ask the user where the wiki should live and create `raw/`, `wiki/`, `wiki/index.md`, and a schema file before proceeding.

## Mode: $ARGUMENTS

- **ingest** — Read the new source named in the arguments, then update the relevant wiki pages (entity pages, topic summaries, the index). Flag anything that contradicts what's already there.
- **query** — Check `wiki/index.md` first, then the pages it points to, and answer from what the wiki already knows. Don't start from the raw sources unless the wiki is silent on the question.
- **lint** — Health-check the wiki: orphan pages, stale claims, missing cross-references. Report findings; don't fix silently.

If no mode is given, ask the user which of the three they want.
