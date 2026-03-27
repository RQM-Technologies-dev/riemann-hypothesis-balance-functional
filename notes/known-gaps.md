This page exists to make mathematical scrutiny easier.

# Known Gaps (Audit-Facing)

This register tracks the simplified manuscript built around one canonical object:
\[
\Phi(q):=\Gamma(q)(1-q)\zeta(q).
\]

Editorial status note (2026-03-27): the manuscript main flow was simplified to one object, one balance notion, and one exclusion target. This simplification is intentional and does not close any major proof gap by itself.

Conventions:
- **Status labels:** Open / Partial / Blocked.
- **Resolution criterion:** what would count as mathematical closure.
- **Evidence rule:** computational or heuristic evidence can guide work but does not prove theorems.

---

## 1) Why this \(\Phi\) is the canonical object

**Gap:** The manuscript chooses
\[
\Phi(q)=\Gamma(q)(1-q)\zeta(q)
\]
as the main-text balance object, but this choice is a simplifying decision under audit, not a uniqueness theorem.

**Why it matters:**
- The proof spine depends on this one definition.
- If the choice is poorly scoped, later targets may not be the right reduction route.

**Current status:** **Open (foundational framing).**

**What would count as resolution:**
- A precise theorem-level justification that this \(\Phi\) is sufficient for the intended RH reduction route.
- Clear domain statements and non-circular assumptions for all uses of \(\Phi\).

---

## 2) Zero correspondence for the chosen balance condition

**Gap:** The manuscript target is to prove strip-level correspondence between
\[
\Phi(q)=0
\quad\text{and}\quad
\zeta(q)=0 \text{ (nontrivial zeros)}.
\]
This theorem is not yet proved in full manuscript detail.

**Why it matters:**
- Target A is the first essential bridge in the proof spine.
- Without exact correspondence, the RH reduction cannot proceed.

**Current status:** **Open (critical).**

**What would count as resolution:**
- A complete two-direction theorem with explicit hypotheses and domain.
- Proof that no spurious strip-balanced points are introduced by the chosen formulation.

---

## 3) Critical condition: why balance forces \(\Re(q)=1/2\)

**Gap:** The central exclusion target
\[
\Phi(q)=0 \Rightarrow \Re(q)=\tfrac12
\]
on the strip remains open.

**Why it matters:**
- This is Target B in the simplified manuscript.
- RH requires exclusion of all off-line strip candidates.

**Current status:** **Open (central).**

**What would count as resolution:**
- A theorem-level critical-line exclusion proof under one synchronized hypothesis package.
- Explicit control of all strip regimes used in the argument.

---

## 4) Global exclusion from local arguments (if used)

**Gap:** Any local-to-global transfer used to support Target B must be proved explicitly.

**Why it matters:**
- Local control alone does not settle strip-wide exclusion.
- Hidden assumptions can enter at continuation/extension steps.

**Current status:** **Open (technical).**

**What would count as resolution:**
- A complete theorem that upgrades local exclusion to strip-wide exclusion under declared assumptions.
- Proof-level justification of all continuation/interchange operations used.

---

## 5) Heuristic vs theorem boundary

**Gap:** Some motivation remains heuristic.

**Why it matters:**
- Heuristic interpretation cannot replace theorem-level proof.

**Current status:** **Partial.**

**What would count as resolution:**
- Every RH-relevant step written as theorem + proof under explicit hypotheses.
- Heuristic remarks kept clearly labeled and non-essential.

---

## At-a-glance risk board

| Gap | Why it matters (short) | Status | Resolution signal |
|---|---|---|---|
| Canonical \(\Phi\) justification | Foundational scope of the spine | Open | Theorem-level sufficiency/justification |
| Target A (zero correspondence) | Links balance to zeta zeros | Open | Two-direction correspondence theorem |
| Target B (critical-line exclusion) | Excludes off-line balanced points | Open | Strip-wide exclusion theorem |
| Local-to-global transfer | Prevents regime gaps | Open | Full transfer theorem |
| Heuristic/theorem separation | Protects rigor | Partial | Explicit formal replacements |

---

## Reviewer use

This file is intended to answer:
1. Which bridges are still open?
2. Are they acknowledged explicitly?
3. What exact theorem milestones would close them?

*Last updated: 2026-03-27.*
