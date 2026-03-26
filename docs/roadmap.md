# Roadmap

*Operational sequencing for publication and formalization of this proposed proof framework.*

This roadmap is designed to support real go/no-go decisions. It separates:
- **Outputs** (what artifacts should exist),
- **Dependencies** (what must already be true),
- **Completion criteria** (what counts as ready).

Timing remains intentionally noncommittal. Movement between phases is governed by mathematical readiness, not momentum.

---

## Current repository baseline (as of 2026-03-26)

The repository already contains:
- A full manuscript file structure in `manuscript/`.
- Audit-oriented documentation in `docs/` (claim map, notation, FAQ, overviews, roadmap).
- Gap-tracking and objection-tracking notes in `notes/`.
- Supporting workflows for LaTeX build and link checking in `.github/workflows/`.
- Early computational notebooks in `code/notebooks/`.

The repository does **not** yet claim a stable proof state. Core bridges remain open in `notes/known-gaps.md`, and the review log currently reports no external expert feedback received.

---

## Phase 1 — Clean Public Repository *(current stage)*

### Outputs
- Public repository organized for mathematical audit.
- Core navigation documents (`README.md`, `docs/claim-map.md`, `docs/notation.md`, `docs/faq.md`, overviews).
- Baseline issue templates and CI workflows that support review quality.
- Initial notes for known gaps, objections, and review logging.

### Dependencies
- None beyond maintaining a coherent repository structure.

### Completion criteria
Phase 1 is complete when all of the following are true:
1. The repository can be read end-to-end as an audit package without missing structural files.
2. `notes/known-gaps.md` and `notes/objections-and-responses.md` are substantively populated (not placeholders).
3. The manuscript compiles through CI in its current form.
4. Current limitations are visible and not contradicted by audience-facing docs.

### Practical status
- **In progress, near completion.** Structure and core documents are present, and gap/objection notes are populated.
- The remaining practical check is consistency hardening: verify that all docs, manuscript caveats, and status statements remain aligned after each substantive edit.

---

## Phase 2 — Stable Manuscript

### Outputs
- A manuscript where definitions, claims, and unresolved bridges are consistently labeled.
- A dependency-consistent claim flow across `manuscript/*.tex`.
- Explicitly marked placeholders wherever proofs are still missing.
- Updated `notes/known-gaps.md` mapping each open bridge to its manuscript location.

### Dependencies
- Phase 1 completion.
- Foundational operator-definition decisions sufficient to keep statements internally consistent, even if some bridges remain open.

### Completion criteria
Phase 2 is complete when all of the following are true:
1. Every theorem/proposition-level claim has explicit hypotheses and a clear dependency path.
2. Every non-proven bridge is marked in-manuscript and mirrored in `notes/known-gaps.md`.
3. No section implicitly treats heuristic language as proof.
4. Cross-references, notation, and terminology are internally consistent across manuscript and docs.
5. CI builds the manuscript without unresolved structural errors.

### Practical status
- **Not yet complete.** Manuscript breadth exists, but central bridges are still open (operator definition, correspondence theorem, uniqueness/exclusion steps).

---

## Phase 3 — Code and Visual Support

### Outputs
- Reproducible notebooks and scripts that generate manuscript-facing figures.
- Documentation of computational assumptions and limits.
- A clear boundary statement that computations support intuition/audit but do not establish proof.

### Dependencies
- Phase 2-level notation and claim stability (so figures correspond to stable definitions).
- Minimal reproducibility instructions in `code/README.md`.

### Completion criteria
Phase 3 is complete when all of the following are true:
1. Notebooks run from a clean environment using documented steps.
2. Figures used by manuscript/docs are generated programmatically and traceable to source code.
3. Computational outputs are linked to specific claims as supporting evidence only.
4. Any numerical limitations (precision, range, sampling, instability) are explicitly documented.

### Practical status
- **Early partial state.** Notebook files exist, but reproducibility and claim linkage should be treated as pending until explicitly documented.

---

## Phase 4 — Private Expert Review

### Outputs
- A review packet suitable for domain experts (manuscript + claim map + known gaps).
- External feedback records in `notes/review-log.md`.
- A response cycle reflected in `notes/objections-and-responses.md` and manuscript edits.

### Dependencies
- Phase 2 completion (stable manuscript baseline).
- At least minimally reproducible Phase 3 outputs if computational evidence is referenced.

### Completion criteria
Phase 4 is complete when all of the following are true:
1. At least two qualified expert reviewers have provided substantive feedback (private correspondence or public issue comments).
2. Each substantive critique is logged and assigned a disposition: accepted, partially addressed, or open.
3. Revisions are documented with explicit pointers to changed sections.
4. Remaining unresolved critiques are visible rather than silently dropped.

### Practical status
- **Not started.** Review log currently indicates no external reviews recorded.

---

## Phase 5 — Public Archival Release

### Outputs
- A versioned repository release suitable for citation.
- DOI-backed archival snapshot (e.g., Zenodo).
- Public preprint artifact (if pursued) with status language consistent with manuscript limitations.

### Dependencies
- Phase 4 completion with review-informed revisions incorporated or explicitly deferred.
- `CITATION.cff` updated for archival identifiers.

### Completion criteria
Phase 5 is complete when all of the following are true:
1. A tagged release corresponds to a specific, review-traceable manuscript state.
2. DOI metadata resolves correctly and matches repository citation files.
3. Any public abstract/description preserves uncertainty and open-bridge disclosures.
4. Archival artifacts are internally consistent (version, date, citation identifiers).

### Practical status
- **Not started.** No DOI/arXiv archival identifiers are currently recorded.

---

## Phase 6 — Journal Submission

### Outputs
- Journal-formatted manuscript package.
- Submission documents (cover letter, metadata, supplementary notes if needed).
- Internal record of submission state and reviewer correspondence.

### Dependencies
- Phase 5 completion.
- A manuscript state the author is prepared to defend under formal peer review, including explicit handling of any unresolved claims.

### Completion criteria
Phase 6 is complete when all of the following are true:
1. Target journal scope matches the manuscript’s technical content and current evidence level.
2. Submission package passes journal formatting and policy checks.
3. Any unresolved bridge is disclosed in language compatible with editorial standards.
4. Submission date, venue, and manuscript version are recorded in repo notes.

### Practical status
- **Future phase.** This remains downstream of external review and archival readiness.

---

## Readiness gates

These gates are stricter transition checks. They are intended to prevent premature advancement.

### Gate to **stable manuscript**
Move forward only if:
- Core definitions and assumptions are explicit and consistent.
- Every major claim is categorized as proven / heuristic / open bridge.
- Open bridges are visible both in-manuscript and in `notes/known-gaps.md`.
- CI manuscript build is reliable.

### Gate to **private expert review**
Move forward only if:
- The manuscript is readable without informal oral context.
- Claim dependencies are traceable from `docs/claim-map.md` into manuscript sections.
- Reviewer packet includes known gaps and explicit limitations.
- The author can point reviewers to highest-risk bridges directly.

### Gate to **archival release**
Move forward only if:
- External review has occurred and responses are documented.
- The archived version has a stable citation identity (tag + DOI metadata).
- Public-facing language stays audit-oriented and does not overclaim certainty.
- Versioned artifacts (repo, manuscript PDF, citation metadata) agree.

### Gate to **journal submission**
Move forward only if:
- The manuscript state is coherent under adversarial peer review.
- Major objections have either formal resolutions or explicit limitation statements.
- Evidence type boundaries are clear (formal proof vs. computational support).
- Submission package is complete and repository records the submitted state.

---

## Notes on cadence

No fixed schedule is imposed. A slower phase transition is preferred to advancing with unresolved structural ambiguities. The roadmap should be revised whenever a major claim changes status, a foundational dependency is added, or expert feedback materially alters the proof architecture.
