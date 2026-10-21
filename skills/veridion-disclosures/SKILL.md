---
name: veridion-disclosures
description: Look up U.S. congressional, executive-branch (OGE) and SEC Form 4 trading disclosures with government receipts. Use when the user asks what a member of Congress, an executive-branch official or a company insider bought or sold, or asks for a filing's receipt.
---

# Veridion disclosures

1. Resolve the filer first with `list_members` when the user gives a name.
2. Query `search_disclosures` with the narrowest filters you have (filer, ticker, date range).
3. For one filing's full history, including amendments, use `get_disclosure_history`.
4. Answer only from returned rows, and give the receipt link for each row.
5. If nothing is returned, say that no served rows matched. That is not proof that no filing exists. `get_status` reports source freshness.
