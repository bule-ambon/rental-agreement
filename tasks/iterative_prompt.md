# Iterative Prompt: Lease Topic Coverage Review

You are an AI coding assistant. Review the current lease draft and compare it against the three sample lease documents to identify topic coverage gaps. Keep the output concise, deduplicated, and focused on topics (not exact clauses).

## Files to review
- Draft to analyze: `drafts/agreement.md`
- Sample 1: `Residential_Lease_Agreement for Max & Becca.docx`
- Sample 2: `2019-05 Osborne Properties Residential Lease Template.docx`
- Sample 3 ("sulawesi house" reference): `Tayloe House lease_agreement 4-1-21 for 3 Months.pdf`

## Task
1. Read `drafts/agreement.md` and each sample agreement.
2. Extract the distinct topics covered by each document (examples: renewal terms, late fees, HOA rules, access, holdover).
3. Consolidate overlapping topics so each appears only once.
4. Categorize the topics into the sections below.

## Required output format
Provide a markdown document with the following sections and bullet lists:

A) Topics handled in `drafts/agreement.md` AND all three sample agreements
- ...

B) Topics handled in `drafts/agreement.md` only
- ...

C) Topics handled in `Residential_Lease_Agreement for Max & Becca.docx` only
- ...

D) Topics handled in `2019-05 Osborne Properties Residential Lease Template.docx` only
- ...

E) Topics handled in the "sulawesi house" agreement only (`Tayloe House lease_agreement 4-1-21 for 3 Months.pdf`)
- ...

## Notes
- Do not rewrite the lease. Focus on comparing topic coverage.
- Prefer short, clear topic phrases over long sentences.
- If a topic appears in two samples but not the third, do not put it in section A; include it in the relevant sample-only sections.
- If a topic appears in multiple samples but not in `drafts/agreement.md`, list it under each applicable sample-only section.
