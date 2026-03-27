This register is maintained for mathematical audit.

# Known Gaps (Simplified Proof Spine)

The manuscript is organized around
\[
\Phi(s):=\Gamma(s)(1-s)\zeta(s).
\]

Editorial status note (2026-03-27): the draft was compressed to one direct proof spine. This improves traceability but does not close the central theorem gap.

Conventions:
- **Status labels:** Open / Partial / Blocked.
- **Resolution criterion:** theorem-level closure under explicit hypotheses.
- **Evidence rule:** heuristic or computational evidence is supportive, not a proof substitute.

---

## 1) Strip correspondence bookkeeping

**Gap:** The strip correspondence
\[
\Phi(s)=0\iff\zeta(s)=0
\quad (0<\Re(s)<1)
\]
is straightforward, but the manuscript still needs consistent bookkeeping in every use (domain restrictions, exclusion of poles, and explicit strip hypotheses).

**Status:** **Partial (technical clarity).**

**Resolution criterion:**
- Every theorem or lemma invocation states the strip hypothesis explicitly.
- No step applies the correspondence outside its valid domain.

---

## 2) Critical-line exclusion from the raw zero condition

**Gap:** The core theorem target is still open:
\[
0<\Re(s)<1,\ \Phi(s)=0
\Longrightarrow
\Re(s)=\tfrac12.
\]

**Status:** **Open (central).**

**Resolution criterion:**
- A complete proof under a single coherent hypothesis package.
- Explicit exclusion of off-line strip points.

---

## 3) RH closure from the core target

**Gap:** RH follows conditionally once Item 2 is proved, but unconditional closure is unavailable because Item 2 is open.

**Status:** **Open (depends on Item 2).**

**Resolution criterion:**
- Closure of Item 2.
- Final theorem statement with dependencies and hypotheses fully documented.

---

## Reviewer quick check

This file now tracks three direct checks:
1. Is strip correspondence used with correct domain restrictions?
2. Is critical-line exclusion proved from \(\Phi(s)=0\)?
3. If not, is RH correctly presented as conditional only?

If Item 2 is unresolved, RH remains unproved in this manuscript.

*Last updated: 2026-03-27.*
