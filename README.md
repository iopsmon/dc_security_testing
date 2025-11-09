# Security Testing & Monitoring Toolkit

A collection of non-destructive Linux / Splunk operational checks, pen-test command templates, and monitoring lookup exports. Intended as a practical reference for authorised security testing, Splunk monitoring development and operational runbooks.

## Contents
- Guides and cheat-sheets (HTML) for quick copy/paste
- Bash script templates and TLS helpers
- Git / Linux command cheat sheets
- Pen-test command templates and a CSV lookup for Splunk ingestion

## Quick start
1. Open the HTML guides in your browser (examples):
   - Pen-test guide: `WEB_DEV/HTML/dc_linux_pen_test.html`  
     (Windows path example: `d:\LOCAL\HOME_LAB_DOCS\WEB_DEV\HTML\dc_linux_pen_test.html`)  
     Click the link or open the file in your browser to view commands and copy-to-clipboard buttons.
2. To use checks in Splunk:
   - Export or download the provided CSV lookup (see the "CSV Lookup / Monitoring Export" section in the pen-test HTML).
   - In Splunk: Settings → Lookups → Add lookup table file → upload the CSV, then use `| inputlookup <lookupname>` in searches.
3. Add your scripts and notes in the appropriate HTML pages or in `/SCRIPTING` and commit changes.

## Recommended workflow
- Test commands in a lab or containerised environment before running in production.
- Do not store plaintext secrets in repo files; use a secrets manager or environment variables with strict permissions.
- Use the CSV lookup to drive scheduled Splunk checks or dashboards for continuous monitoring.

## Contribution
- Add new commands or sections via pull requests.
- Keep each snippet documented with purpose, required privileges and non-destructive notes.
- Use sensible filenames and keep HTML guides in `WEB_DEV/HTML/`.

## License & Use
For internal use. Obtain written authorization before running any penetration tests. Modify and extend for local procedures.
