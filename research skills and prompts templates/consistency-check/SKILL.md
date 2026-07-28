---
name: consistency-check
description: Checks a proposal for formatting consistency (fonts, headings, table/figure numbering, section numbering) and citation-style consistency, then offers to convert the reference list to a target style. Pass the citation style to check against.
argument-hint: [citation style, e.g. APA / Vancouver / IEEE]
disable-model-invocation: true
---

# Consistency Check

Ask the user to paste or attach the proposal if it isn't already in the conversation. Citation style to check against: **$ARGUMENTS** (if not given, ask the user which style before proceeding).

Check the proposal for consistency:

- Fonts and heading styles.
- Table and figure numbering and captions.
- Section numbering.
- Every reference against the named citation style — flag any that don't match.

Offer to convert the whole reference list to a different target style if the user asks.
