# AIA Pay Application Toolkit

A practical, open toolkit for understanding and working with **AIA-style G702 & G703 pay applications**.  
This repository is intended for contractors, project managers, office administrators, and developers who want clear, accurate references for construction progress billing workflows.

> **Not affiliated with the American Institute of Architects (AIA).**  
> AIA®, G702®, and G703® are registered trademarks of the American Institute of Architects.

---

## What This Repo Is

This project provides **plain-English explanations, examples, and technical references** for how AIA-style pay applications work — without requiring proprietary forms or licensed PDFs.

Use this repo to:
- Understand how G702 summaries and G703 continuation sheets work
- Learn how Schedule of Values (SOV) data is structured
- Reference retainage and progress billing calculations
- Avoid common pay application mistakes that cause rejections or delays

---

## What This Repo Is Not

- Not a replacement for licensed AIA forms
- Not a full billing system or PDF generator
- Not legal or accounting advice

If you need a production-ready, hosted solution with PDFs, approvals, history, and compliance checks, see **Related Tools** below.

---

## Repository Structure

<details>
<summary><strong>View folder layout</strong></summary>

- `/`
  - `docs/` — educational references
    - `what-is-aia-g702-g703.md`
    - `schedule-of-values-explained.md`
    - `common-pay-app-mistakes.md`
    - `retainage-explained.md`
  - `examples/` — sample data files
    - `g703-continuation-sheet-example.csv`
    - `g703-continuation-sheet-example.json`
    - `sample-sov.csv`
    - `g702-summary-totals-example.json`
  - `schemas/` — data structure references
    - `pay-application.schema.json`
  - `calculations/` — billing logic notes
    - `retainage-math.md`
    - `progress-vs-final-billing.md`
    - `stored-materials-notes.md`
  - `README.md`

</details>

---

## Key Concepts Covered

### G702 (Application and Certificate for Payment)
- Summary-level view of the pay application
- Totals pulled from the G703 continuation sheet
- Typically signed by the contractor and architect/owner

### G703 (Continuation Sheet)
- Line-item detail based on the Schedule of Values
- Tracks:
  - Work completed to date
  - Stored materials
  - Retainage
  - Previous vs current billing

### Schedule of Values (SOV)
- Backbone of every pay application
- Defines how contract value is broken into billable components
- Errors here cascade through the entire billing cycle

---

## Common Problems This Repo Helps Prevent

- Overbilling beyond line-item contract value
- Incorrect retainage calculations
- Confusion between work completed and materials stored
- Rejected pay apps due to math inconsistencies
- Misaligned progress vs final billing totals

---

## Who This Is For

- Subcontractors new to AIA billing
- Project managers reviewing pay apps
- Office administrators handling monthly draws
- Developers building construction billing tools
- Anyone tired of guessing how G703 math works

---

## Related Tools

If you are looking for a **hosted, production-ready pay application builder** with:
- Automated G702/G703 calculations
- Schedule of Values management
- PDF exports
- Lien waiver and compliance workflows

You may want to look at **PayAppPro**:  
https://payapppro.com

PayAppPro is built specifically for subcontractors and contractors who submit AIA-style pay applications regularly.

---

## Contributions

Contributions are welcome.

Helpful additions include:
- Clearer documentation
- Edge-case billing scenarios
- Example data sets
- Calculation explanations

Please open an issue or submit a pull request.

---

## Disclaimer

This repository is provided for **educational and reference purposes only**.

Always consult your contract documents, owner requirements, and licensed professionals when submitting pay applications.

---

## License

MIT License.  
See `LICENSE` file for details.
