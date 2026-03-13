# EG2 Public Note

The `EG2` package establishes admissible capture across deformation and restart.

Raw theorem constant:

`sigma_sparsity^(raw) := sparsity_floor_raw - truncation_loss_raw - restart_loss_raw`.

Closure criterion:

- the admissible defect ledger remains above the declared capture floor,
- restart losses are explicitly budgeted,
- the canonical transport remains inside the admissible tube.

Main interpretation: the tracked sparsity defect does not consume the full closure budget.
