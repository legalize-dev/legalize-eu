# legalize-eu

European Union legislation in Markdown, version-controlled as a git repository.

Each law is a file; each reform is a commit dated to the real official publication date. The `git log` of any law shows its full history — when it was enacted, which articles changed and by which norm.

Selected EU institutional legislation with English HTML/XHTML originals in CELLAR: regulations, directives, decisions and international agreements. Published laws are retained; additions are qualified by source accessibility and supported formats. National legislation is outside this corpus. Histories include the original publication and available consolidated snapshots. Unconsolidated amended acts retain their as-enacted body and record actual amending acts separately.

## What's inside

- **Regulation** (`3YYYYRNNNN.md`) — `eu/6e/32016R0679.md`, `eu/fb/32014R0596.md`, `eu/e0/32024R1689.md`
- **Implementing Regulation** (`3YYYYRNNNN.md`) — Commission implementing regulations (resource type REG_IMPL). The source resource type is retained in frontmatter extra.resource_type.
- **Delegated Regulation** (`3YYYYRNNNN.md`) — Commission delegated regulations (resource type REG_DEL).
- **Financial Regulation** (`3YYYYRNNNN.md`) — Financial regulations (resource type REG_FINANC).
- **Directive** (`3YYYYLNNNN.md`) — Selected directives with supported English source histories.
- **Decision** (`3YYYYDNNNN.md`) — Selected decisions with supported English source histories.
- **International agreement** (`2YYYYANNNN(NN).md`) — Selected international agreements with supported English source histories.

## Data source

- **EUR-Lex / CELLAR — Publications Office of the European Union**
  - Portal: https://eur-lex.europa.eu
  - SPARQL endpoint (CELLAR): https://publications.europa.eu/webapi/rdf/sparql
  - REST API (CELLAR): https://publications.europa.eu/resource/cellar/
  - Consolidated texts: https://eur-lex.europa.eu/collection/eu-law/consleg.html
  - Reuse and authenticity: https://eur-lex.europa.eu/content/legal-notice/legal-notice.html?locale=en

## Attribution

> © European Union, https://eur-lex.europa.eu — Source: EUR-Lex (Publications Office of the European Union). EU-owned consolidated texts are reused under CC BY 4.0; metadata is available under CC0 1.0. This reformatted corpus is not an official publication. Consolidated texts have no legal effect; consult the authentic Official Journal edition.

## Coverage and limitations

- **English source texts.** Other official languages are outside this reconstruction. The catalogue is a measured selection, not complete EU-law coverage.
- **Published and effective dates differ.** Original Git author dates and Source-Date use official publication. A consolidation date is its applicability date; when it has no official publication date, Source-Date is omitted and the base publication supplies the Git author-date fallback. A qualified future commencement is retained as the date of that point-in-time text.
- **Historical PDF sources.** Text-layer PDF/PDF-A snapshots can be extracted. Scans, unsafe font encodings and inaccessible versions fail normal processing. Reviewed local draft exclusions are recorded in each law's extra.source_version_gaps and do not constitute complete history.
- **Images.** Drawings, formulas and image-based forms remain at the official source. Omission markers link to that source; an HTML wrapper does not prove that every annex is machine-readable text. Optional catalogue additions with unreviewed images are excluded. Required amending-act files are retained with visible source links and documented visual omissions.
- **As-enacted texts.** Their amendments are not incorporated into the body. Required amending acts whose source or legal-status metadata cannot be qualified remain a documented coverage gap; this must be reconciled before publication.
- **Identifiers and paths.** CELEX supplies the identifier. Resolve file paths from .legalize.yml; paths are sharded by identifier hash. Source properties, multiplicity and qualified date annotations are retained in extra.source_metadata.
- **No snapshot cap.** Available historical versions are retained rather than truncated to the latest 200.

## Other countries

This repository is part of **Legalize**, which maintains the legislation of multiple countries as git repos. See https://legalize.dev for the full catalog.

## Support

Legalize is free and open. If this work is useful to you, you can help sustain its hosting and development: [Support this project](https://buymeacoffee.com/legalizedev).

## License

- **Pipeline code**: MIT (https://github.com/legalize-dev/legalize-pipeline)
- **Data**: EUR-Lex consolidated texts and EU-owned editorial content: CC BY 4.0; EUR-Lex metadata: CC0 1.0. See the official legal notice and any document-specific restrictions.
