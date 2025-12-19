# Retainage Math Explained

Retainage is one of the most common sources of pay application errors.  
The math itself is simple, but mistakes happen when retainage is applied inconsistently or summarized incorrectly.

This document explains **how retainage math typically works in AIA-style billing**, with a focus on clarity and consistency rather than contract-specific rules.

---

## What Retainage Is (Quick Recap)

Retainage is a percentage of the value of work completed that is:
- Withheld from each progress payment
- Accumulated over the life of the project
- Released later, usually at substantial or final completion

Typical retainage rates range from **5% to 10%**, depending on the contract.

---

## Where Retainage Is Calculated

In AIA-style workflows, retainage should be applied:

1. **At the line-item level (G703)**
2. Then **summarized at the application level (G702)**

Applying retainage only at the summary level often causes rounding errors and mismatches.

---

## Line-Item Retainage (G703)

For each line item:

1. Determine the **total completed and stored to date**
2. Apply the retainage percentage
3. Subtract retainage to arrive at **net earned**

Conceptually:

- Retainage (to date) = Completed & Stored × Retainage %
- Net Earned (to date) = Completed & Stored − Retainage

Each line item carries its own retainage balance.

---

## Summary Retainage (G702)

At the summary level:

- Retainage to date is the **sum of line-item retainage**
- Net earned to date is the **sum of line-item net earned values**
- Current payment due is calculated after subtracting prior payments

The G702 does not create retainage — it only summarizes what already exists on the G703.

---

## Prior vs Current Period Retainage

Retainage accumulates over time.

Each application includes:
- Retainage held from prior periods
- Retainage generated in the current period
- Total retainage held to date

Confusing these amounts is a common cause of rejected applications.

---

## Retainage and Percent Complete

Percent complete and retainage are related but independent:

- Percent complete measures progress against the scheduled value
- Retainage measures withheld dollars

Errors occur when percent complete is adjusted without reconciling retainage totals.

---

## Retainage Changes Mid-Project

Some contracts allow:
- Retainage reduction after a completion threshold
- Partial release at substantial completion

When retainage rules change:
- Previously withheld retainage remains held unless explicitly released
- New work is subject to the new retainage rate
- Consistency across all line items is critical

Retainage changes should never be applied retroactively without documentation.

---

## Retainage and Stored Materials

Stored materials may be:
- Subject to full retainage
- Subject to reduced retainage
- Excluded from retainage entirely

The treatment depends on the contract and owner requirements.

Stored materials should:
- Be tracked separately from installed work
- Follow the same retainage rules consistently
- Be clearly documented to avoid disputes

---

## Common Retainage Math Errors

- Applying retainage only at the summary level
- Inconsistent retainage percentages across line items
- Forgetting to update retainage after approved reductions
- Rounding line items differently than totals
- Manually editing G702 retainage without reconciling G703 values

Most retainage issues are arithmetic, not contractual.

---

## Best Practices

- Apply retainage at the line-item level
- Let summary totals roll up naturally
- Avoid manual overrides
- Reconcile retainage every billing cycle
- Document retainage changes clearly

Consistency matters more than speed.

---

## Related Examples

See the following files for practical reference:
- `examples/g703-continuation-sheet-example.csv`
- `examples/g702-summary-totals-example.json`
- `docs/retainage-explained.md`

---

## Disclaimer

This document is provided for educational and reference purposes only.  
Always follow your contract documents and owner requirements when applying retainage.
