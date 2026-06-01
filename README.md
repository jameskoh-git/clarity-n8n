# Clarity n8n

Clarity is an AI/n8n-powered real estate operating system for a Singapore real estate team.

Core architecture:

Boss Sheets (read-only)
→ Clarity V2 Central Database (writable)
→ n8n workflows
→ Google Docs / Drive outputs / reports

## Safety Rules

- Boss sheets are read-only.
- Automation must never write to Master Listing Sales or Master Listing Rentals.
- Only Clarity V2 central sheets are writable.
- n8n workflows must default to inactive unless manually approved.
- Do not use alexgohassociates@gmail.com credentials for automation.
- Use jameskoh.kjk@gmail.com credentials for Clarity workflows.
