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
