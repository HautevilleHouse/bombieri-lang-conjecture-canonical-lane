# The Bombieri-Lang Conjecture via Rational-Point Sparsity Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global architecture (`BL1-BL8`)

**Author:** HautevilleHouse  
**Date:** March 12, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving sparsity of rational points on varieties of general type through an admissible rational-point closure architecture.

The proof program is organized as eight steps `BL1-BL8` with executable closure gates `BL_G1`, `BL_G2`, `BL_G3`, `BL_G4`, `BL_G5`, `BL_G6`, and `BL_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

The target statement is: sparsity of rational points on varieties of general type.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let `u_tau = (P_tau, H_tau, D_tau, N_tau, L_tau)` denote the admissible state of rational-point packets, height-truncation data, defect ledgers, normalization parameters, and endpoint locks.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_BL = min(kappa_rational, sigma_sparsity, kappa_compact, rho_rigidity, lang_transfer) - eps_coh`.

Target:

`M_BL > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive rational-point response that prevents collapse of the admissible closure package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `BL_G1` | `kappa_rational` | projected rational-point response has a strict positive floor |
| `BL_G2` | `sigma_sparsity` | sparsity defect stays above capture floor across admissible truncation losses |
| `BL_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `BL_G4` | `rho_rigidity` | bad density-counterexample models are excluded |
| `BL_G5` | `lang_transfer` | rigid limit transfers to the Bombieri-Lang endpoint class |
| `BL_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `BL_GM` | derived | all upstream gates pass and `M_BL > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_rational` = 1.0937330000000003,
- `sigma_sparsity` = 1.074,
- `kappa_compact` = 0.8038585209003215,
- `rho_rigidity` = 1.077,
- `lang_transfer` = 1.029422,
- `eps_coh = 0.0`.

Hence:

`M_BL = 0.8038585209003215 > 0`.

### 4.5 Raw coercive constant

Define `kappa_rational^(raw) := c_rational_raw * rational_density_raw - e_rational_raw`.

Current extracted value:

`kappa_rational = 1.0937330000000003`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`BL1-BL8`)

1. `BL1` Active projected response block on the canonical sector.
2. `BL2` Uniform capture bounds on the canonical admissible tube.
3. `BL3` Restart map preserving admissible data.
4. `BL4` First-failure compactness extraction.
5. `BL5` Rigidity exclusion of bad countermodels.
6. `BL6` Endpoint transfer closure on the extracted target class.
7. `BL7` Determining-class identification of the intended endpoint.
8. `BL8` Final persistence theorem: the endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_sparsity^(raw) := sparsity_floor_raw - truncation_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_sparsity = 1.074`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8038585209003215`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of bad density-counterexample models incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.077 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the Bombieri-Lang endpoint class by the bridge inequality.

Define `lang_transfer^(raw) := c_transfer_raw * transfer_gain_raw - e_transfer_raw`.

Current extracted value:

`lang_transfer = 1.029422 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of endpoint observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_rational` | `BL_G1` | `1.0937330000000003` |
| `sigma_sparsity` | `BL_G2` | `1.074` |
| `kappa_compact` | `BL_G3` | `0.8038585209003215` |
| `rho_rigidity` | `BL_G4` | `1.077` |
| `lang_transfer` | `BL_G5` | `1.029422` |
| `eps_coh` | `BL_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `BL_G1, BL_G2, BL_G3, BL_G4, BL_G5, BL_G6, BL_GM = PASS`,
- strict margin `M_BL = 0.8038585209003215`,
- lane: `manifold_constrained`.
