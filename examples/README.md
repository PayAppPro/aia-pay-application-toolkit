# Example Files

This folder contains **illustrative, AIA-style reference examples** intended to demonstrate how pay application data is commonly structured, calculated, and rolled up.

These files are **not licensed AIA forms** and are provided for **educational and reference purposes only**.

---

## g703-continuation-sheet-example.csv

A realistic, internally consistent example of a **G703-style continuation sheet**.

Key characteristics:
- Line items based on a typical commercial construction project
- Includes prior work, current period work, and materials presently stored
- Uses a **10% retainage rate** (common, but contract-dependent)
- Demonstrates partial, full, and zero-completion line items
- All math is internally consistent for validation and testing

Intended uses:
- Reference for understanding G703 structure and columns
- Import testing for billing software
- Math validation and reconciliation examples

---

## sample-sov.csv

A simplified **Schedule of Values (SOV)** derived from the same line items used in the G703 example.

Key characteristics:
- Clean, import-friendly structure
- Totals exactly to the contract value
- Matches the G703 line items one-to-one

Intended uses:
- SOV setup reference
- Import and onboarding examples
- Understanding how SOV values roll into G703 and G702 calculations

---

## g703-continuation-sheet-example.json

A JSON representation of the same G703-style data shown in the CSV example.

Key characteristics:
- Mirrors the CSV line items and values
- Uses predictable, developer-friendly field names
- Includes calculated fields such as percent complete, retainage, and net earned

Intended uses:
- Software development reference
- API and data-structure examples
- Programmatic calculation and validation testing

---

## g702-summary-totals-example.json

A **G702-style summary roll-up** derived from the example G703 data.

Key characteristics:
- Aggregates totals from the G703 continuation sheet
- Demonstrates how line-item values roll up into summary-level fields
- Includes retainage, net earned, prior payments, and current payment due
- Clearly documents calculation assumptions

Intended uses:
- Understanding the relationship between G703 and G702
- Testing roll-up logic and reconciliation workflows
- Reference for building or validating pay application summaries

---

## General Notes

- All examples are internally consistent but intentionally simplified
- Totals and assumptions are documented where applicable
- Real-world contracts may apply different retainage rules, material handling, or approval requirements

---

## Disclaimer

These examples are provided for educational and reference purposes only and do not constitute legal, accounting, or contractual advice. Always follow your contract documents, owner requirements, and project-specific instructions.

