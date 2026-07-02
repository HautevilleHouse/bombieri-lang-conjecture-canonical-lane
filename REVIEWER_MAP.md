# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
- Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

## Theorem Dependency Chain

1. `EG1`: coercive response and active control floor.
2. `EG2`: capture and admissible continuation.
3. `EG3`: compactness and no-collapse spacing.
4. `EG4`: rigidity and transfer.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `BL_G1`, `BL_G2`, `BL_G3`, `BL_G4`, `BL_G5`, `BL_G6`, `BL_GM` all `PASS`.

Primary files:

- `paper/BOMBIERI_LANG_CONJECTURE_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `BL_G1` | `kappa_rational` | projected rational-point response has a strict positive floor |
| `BL_G2` | `sigma_sparsity` | sparsity defect stays above capture floor across admissible truncation losses |
| `BL_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `BL_G4` | `rho_rigidity` | bad density-counterexample models are excluded |
| `BL_G5` | `lang_transfer` | rigid limit transfers to the Bombieri-Lang endpoint class |
| `BL_G6` | `eps_coh` | strict coherence / identification closure |
| `BL_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A certified counterexample to any EG theorem statement used in the paper.
