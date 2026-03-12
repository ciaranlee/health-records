# Health Records Repo

Personal health records for Ciaran Lee (DOB 1980-10-26).

## Structure

- `profile.md` — Demographics and baseline info
- `conditions/` — One markdown file per condition/injury, with history, current status, and management approach. Cross-references results and consultations.
- `results/` — Dated medical results (MRI, blood work, scans). Named as `YYYY-MM-DD-description.md`. Referenced from condition files.
- `consultations/` — Dated doctor visit notes. Named as `YYYY-MM-DD-provider-topic.md`. Referenced from condition files.
- `medications/current.md` — Active medications
- `scanned_images/` — Raw scans and photos of medical documents. Referenced from transcribed files in results/ or consultations/.

## Conventions

- All files are markdown
- Dates use ISO format (YYYY-MM-DD)
- Result and consultation files are prefixed with their date
- Condition files link to relevant results and consultations using relative paths
- New conditions, results, or consultations are added as new files in the appropriate directory
- Scanned images stay in `scanned_images/` and are referenced from transcribed files
- Units: use mmol/L for cholesterol, mmHg for blood pressure unless source uses different units
