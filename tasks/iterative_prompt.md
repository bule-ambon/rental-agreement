# Iterative Prompt: Lease Topic Coverage Review

You are an AI coding assistant. Review the current lease draft and compare it against the three sample lease documents to identify topic coverage gaps. Keep the output concise, deduplicated, and focused on topics (not exact clauses).

## Files to review
- Draft to analyze: `drafts/agreement.md`
- Exclusions list: `drafts/leave_out.md`
- Additions list: `drafts/add_in.md`
- Sample 1: `docs/residential_lease_agreement_max_becca.md`
- Sample 2: `docs/osborne_properties_lease_template.md`
- Sample 3 ("sulawesi house" reference): `docs/tayloe_house_lease.md`

## Task
1. Read `drafts/agreement.md`, `drafts/leave_out.md`, `drafts/add_in.md`, and each sample agreement.
2. Extract the distinct topics covered by each document (examples: renewal terms, late fees, HOA rules, access, holdover).
3. Consolidate overlapping topics so each appears only once.
4. Categorize the topics into the sections below.
5. If any topic in `drafts/leave_out.md` appears in `drafts/agreement.md`, flag it under a new section E.
6. If any topic in `drafts/add_in.md` is missing from `drafts/agreement.md`, flag it under a new section F.

## Required output format
Rewrite `drafts/considerations.md` by replacing its contents with the following sections and bullet lists:

A) Topics handled in `drafts/agreement.md` 
- ...

B) Topics handled in `docs/residential_lease_agreement_max_becca.md` only
- ...

C) Topics handled in `docs/osborne_properties_lease_template.md` only
- ...

D) Topics handled in the "sulawesi house" agreement only (`docs/tayloe_house_lease.md`)
- ...

E) Topics from `drafts/leave_out.md` that still appear in `drafts/agreement.md`
- ...

F) Topics from `drafts/add_in.md` that are missing from `drafts/agreement.md`
- ...

## Notes
- Do not rewrite the lease. Focus on comparing topic coverage.
- Prefer short, clear topic phrases over long sentences, but not so brief as to lose important meaning.
- If a topic appears in two samples but not the third, do not put it in section A; include it in the relevant sample-only sections.
- If a topic appears in multiple samples but not in `drafts/agreement.md`, list it under each applicable sample-only section.
- If sections E or F are empty, write "- None" under that section.
