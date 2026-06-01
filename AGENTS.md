# AGENTS.md

These rules apply to all AI/Codex/automation work in this repository.

## Non-negotiable safety rules

1. Never write to boss sheets.
2. Master Listing Sales and Master Listing Rentals are read-only sources.
3. Only Clarity V2 central sheets are writable.
4. Do not use alexgohassociates@gmail.com credentials for automation.
5. Use jameskoh.kjk@gmail.com credentials for Clarity workflows.
6. All n8n workflow JSON files must default to inactive.
7. Do not activate workflows automatically.
8. Do not send WhatsApp messages without explicit human approval.
9. Do not automate logged-in PropertyGuru mobile/contact extraction.
10. Do not pass authenticated PropertyGuru cookies or sessions into crawlers/scrapers.
11. Prefer manual trigger during MVP unless explicitly approved.
12. Use duplicate-safe upsert logic before scaling sync workflows.
13. Keep workflow changes reviewable through GitHub before production use.

## Current architecture

Boss Sheets:
- Master Listing Sales
- Master Listing Rentals

Central writable database:
- Clarity V2 - Central Database
- Property Registry
- Workflow Logs
- Competitor Records
- Transaction Records
- Document Outputs

## Module status

Module 1D is working:
- Syncs all 8 boss sheet tabs into Property Registry
- Filters by Clarity Route
- Uses Source Key for duplicate-safe upsert
- Boss sheets remain read-only
