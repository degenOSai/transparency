# degenOS — public transparency ledger

Receipts, not promises — applied to ourselves.

Every grading artifact degenOS produces (wallet grades, trust-gate verdicts, farm-league
promotions, entry-gate evaluations, caller scoreboards) is snapshotted every 6 hours into a
hash-chained, append-only internal ledger. **This repo publishes the chain head.**

Each entry in `heads.log` is one snapshot: sequence number, UTC timestamp, number of
artifacts hashed, and the chain-head SHA-256. Because every head commits to the entire
history before it, rewriting ANY past grade, promotion, or receipt would change every
subsequent head published here — in a repo we don't control the clocks on.

What this proves: our grades and receipts were computed when we said they were, and
history was never quietly rewritten. What it doesn't prove: that our grades are good —
that's what the public receipt pages are for.

Verification tooling ships at launch.
