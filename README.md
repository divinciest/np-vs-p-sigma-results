# np-vs-p-sigma-results

Canonical, publicly‑announced **σ board** for NP‑Vs‑P‑Σ — the cached total computation of the
community. `announced.json` holds, per (problem, width): the smallest verified circuit **floor**,
the count of distinct **method‑families** at that floor (the σ input), and the record count.

Aggregated from validated records in **np‑vs‑p‑sigma‑buffer** by its `validate-and-merge` Action.
The app reads this file directly (no auth) so any device gets the community's results without
recomputing. Protect `main` and let only the merge bot push.
