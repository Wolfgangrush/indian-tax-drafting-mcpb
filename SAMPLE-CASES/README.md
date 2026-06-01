# Sample Cases — Reviewer Examples

Three anonymised fact patterns. All party names are placeholders.

## Example 1 — cit-appeals-form-35

> *"Use the connector to draft a cit appeals form 35 (Form 35 CIT(A) appeal under Section 246A IT Act). Use anonymised placeholders for party names and figures."*

Tool sequence: list_case_types → get_case_type_format("cit-appeals-form-35") → get_pleading_base → draft → save_draft_as_docx

## Example 2 — itat-appeal-form-36

> *"Use the connector to draft a itat appeal form 36 (Form 36 ITAT appeal under Section 253 IT Act). Use anonymised placeholders for party names and figures."*

Tool sequence: list_case_types → get_case_type_format("itat-appeal-form-36") → get_pleading_base → draft → save_draft_as_docx

## Example 3 — high-court-appeal-section-260a

> *"Use the connector to draft a high court appeal section 260a (HC tax appeal under Section 260A IT Act on substantial question of law). Use anonymised placeholders for party names and figures."*

Tool sequence: list_case_types → get_case_type_format("high-court-appeal-section-260a") → get_pleading_base → draft → save_draft_as_docx

## Notes for the reviewer

- All examples use placeholders.
- No external API keys / accounts required.
- `save_draft_as_docx` requires `pandoc`.
- Three-layer privacy firewall applies throughout.

---

## Synthetic case folder for Anthropic reviewer

A fully-fictional, AAAK-pseudonymised case folder is bundled at:

`SAMPLE-CASES/synthetic-form-35-cit-appeals-section-14A/`

It contains 3 source documents (.docx) plus a `case-facts-background.md` narrative.

**To exercise the pipeline end-to-end**, point `read_case_folder(path)` at this folder and follow the orchestration script returned by `get_agent_instructions()`. The Reader stage will extract facts, the Format stage will load the case-type SKILL.md template, and the remaining four agents (Drafter → Verifier → Refiner → Overseer) will produce `final-draft.docx`.

All identifiers in the bundled documents are structural placeholders (`[Petitioner-A]`, `[Premises-Address-Placeholder]`, `[Monthly-Rent-Placeholder]`, `[PAN-PLACEHOLDER-10-CHAR]`, `[DIN-PLACEHOLDER-19-DIGIT]`, `[Total-Arrears-Placeholder]`, etc.). The Pseudonymisation Gateway is therefore exercising against pre-pseudonymised content; reviewers seeking to test re-substitution may replace placeholders with their own fictional values before invoking the pipeline.

