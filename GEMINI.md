# Veridion Markets disclosures

The `veridion` MCP server returns U.S. congressional (House and Senate), executive-branch (OGE) and SEC Form 4 disclosure rows. Each row carries a receipt link to the government document it came from.

- Use `search_disclosures` for transactions, `get_disclosure_history` for every recorded version of one filing (amendments included), `list_members` to resolve a filer, `get_coverage` for measured counts and `get_status` for source freshness.
- When you answer, cite the receipt link for each row you use.
- An empty result means no served rows matched. It is not proof that no filing exists.
- Do not estimate amounts, dates or owners that a row does not contain.
