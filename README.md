# Wolfgang Rush — Indian Direct-Tax Appellate Drafting

**MCPB Desktop Extension** for Indian advocates using Claude Desktop App. Local-execution. Zero data collection.

> *Also available as a Claude Code Plugin:* *[github.com/Wolfgangrush/indian-tax-drafting](https://github.com/Wolfgangrush/indian-tax-drafting)*

## What this connector does

Form 35 CIT(A), Form 36 ITAT, Form 10A Section 12A, Section 148A reopening (Ashish Agarwal), 263/264 revision (Malabar Industrial), 271/270A penalty, 144C DRP, 201 TDS, 260A HC. Six-agent local pipeline.

## Case types

- `cit-appeals-form-35` — Form 35 CIT(A) appeal under Section 246A IT Act
- `itat-appeal-form-36` — Form 36 ITAT appeal under Section 253 IT Act
- `high-court-appeal-section-260a` — HC tax appeal under Section 260A IT Act on substantial question of law
- `section-12a-registration-form-10a` — Form 10A Section 12A registration application for charitable trusts
- `section-144c-drp-objection` — Section 144C DRP objection (transfer pricing / corporate)
- `section-148a-reopening-objection` — Section 148A objection in Ashish Agarwal transitional regime
- `section-201-tds-default-reply` — Reply to Section 201 TDS-default order
- `section-263-revision-objection` — Section 263 revision objection on Malabar Industrial twin-condition
- `section-264-revision-application` — Section 264 revision application to PCIT / CIT
- `section-271-270a-penalty-reply` — Section 271 / 270A penalty reply

## Install

1. Claude Desktop App → **Settings → Extensions → Install Extension**
2. Select `wolfgang-indian-tax-drafting.mcpb`
3. Enable

## System requirements

Claude Desktop App ≥ 0.10.0 · Python ≥ 3.10 · `pandoc` for .docx · `pdftotext` for PDF case-files (optional)

## Privacy

Zero data collection. Three-layer privacy firewall. Canonical policy: **<https://wolfgangrush.github.io/privacy/>**


## ⚠️ AI verification disclaimer · 🔒 Pseudonymisation procedure

> **⚠️ AI can make mistakes — please verify the information before filing.**
> Every draft produced by this connector is a STARTING POINT. The Verifier
> agent runs an anti-hallucination firewall and the Overseer agent runs an
> opposing-counsel review, but neither replaces an advocate's independent
> verification of statutory references, citation accuracy, factual fidelity,
> and Registry-formatting compliance with the user's High Court / forum.
> The advocate filing the pleading remains responsible for the contents.
>
> **🔒 Protected by pseudonymisation procedure.** The Reader agent applies a
> domain-specific privacy firewall as the first step of the pipeline — party
> names, addresses, identifying numbers (FIR / CR / Crime / Suit / Diary /
> SLP / lower-court case numbers), PAN / Aadhaar references, financial
> figures, witness names, and statutory-notice references are substituted
> with structural placeholders BEFORE any downstream agent sees the facts.
> The Drafter, Verifier, Refiner, and Overseer agents process placeholders
> only. Real values are re-substituted at the final docx render step on the
> user's local machine. No real identifying data leaves the case folder.

## License

MIT.

## Publisher

**Rushikesh R. Mahajan**, Advocate, Bombay HC Nagpur, publishing as **Wolfgang Rush**. advrushikeshravindramahajan@gmail.com

## Source

<https://github.com/Wolfgangrush/indian-tax-drafting-mcpb>

## Sample cases

See `SAMPLE-CASES/`.
