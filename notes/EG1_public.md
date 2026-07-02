# EG1 Public Note (Projected Response Floor)

Canonical wording: `projection / protected core`.

In-paper anchor: `paper/BOMBIERI_LANG_CONJECTURE_PREPRINT.md` (`BL_G1`).

## Goal
Make the projected response floor explicit as the protected-core gate for `proving sparsity of rational points on varieties of general type through an admissible rational-point closure architecture`.

## Objects

- admissible class: the declared class `A` or routed admissible lattice in the main preprint.
- canonical/base object package: let `u_tau = (P_tau, H_tau, D_tau, N_tau, L_tau)` denote the admissible state of rational-point packets, height-truncation data, defect ledgers, normalization parameters, and endpoint locks.
- projected core: the response sector controlled by `kappa_rational`.
- carried remainder interface: downstream defect and coherence terms remain outside the protected core rather than being hidden in it.

## Closure Criterion

`BL_G1` closes when `kappa_rational` satisfies the response-floor requirement: projected rational-point response has a strict positive floor.
This is the protected-core contribution to the strict margin `M_BL`.

## Lemma Chain and Proof Payload

### Lemma EG1.1 (projection reduction)
On the declared admissible class, the response object may be read on the projected sector without changing the target gate.

Payload: check that all quantities used by `kappa_rational` are defined on the projected sector named in the main preprint.

### Lemma EG1.2 (protected-core floor)
If the projected response floor is positive on the admissible sector, then the core cannot collapse before the later transport and remainder gates are evaluated.

Payload: check the artifact key `kappa_rational` and the corresponding extraction input/provenance record.

### Theorem EG1.3 (core gate closure)
If Lemmas EG1.1-EG1.2 hold and the runtime artifact accepts `kappa_rational`, then `BL_G1` supplies the projected/protected-core input to `M_BL`.

## Current Instantiation

- gate: `BL_G1`
- artifact key: `kappa_rational`
- canonical equivalent: `projection / protected core`
- audit surface: `artifacts/constants_registry.json`, `artifacts/constants_extracted.json`, and `repro/certificate_runtime.json`
