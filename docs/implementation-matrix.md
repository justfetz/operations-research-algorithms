# Implementation Matrix

This matrix shows the current implementation coverage across the public algorithm showcase repos.

| Repo | Problem family | Java baseline | Python baseline | OR-Tools Python | OR-Tools Java | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| `multi-machine-interval-scheduling` | interval scheduling / multi-machine assignment | Yes | Yes | Yes | Yes | Flagship scheduling repo with full parity across the main tracks. |
| `knapsack-and-greedy-algorithms` | 0/1 knapsack, activity selection | Yes | Yes | Yes | Yes | Knapsack has full parity; activity selection is baseline-focused. |
| `python-cutting-stock-operations-research` | 1D cutting stock | Yes | Yes | Yes | No | Strong heuristic plus exact Python model; Java OR-Tools still open. |
| `transportation-and-transshipment-models` | transportation, transshipment | Yes | Yes | Yes | Yes | Greedy route/allocation baselines plus linear optimization parity. |
| `truck-cubing-bin-packing` | bin packing, truck cubing | Yes | Yes | Yes | Yes | Packing lane now has Java, Python, and OR-Tools parity. |
| `network-capacity-transport-planner` | facility capacity planning, regional assignment | Yes | No | No | No | Public-safe repurposing of a real-world capacity planning model with CI and Java regression coverage. |

## Reading the matrix

- `Java baseline` means a plain Java implementation without OR-Tools.
- `Python baseline` means a plain Python implementation without OR-Tools.
- `OR-Tools Python` means a Python optimizer-backed implementation.
- `OR-Tools Java` means a Java optimizer-backed implementation.

## Current gap

The main remaining parity gap in the current public set is:

- `python-cutting-stock-operations-research`
  - Java OR-Tools not added yet
- `network-capacity-transport-planner`
  - Python baseline, OR-Tools Python, and OR-Tools Java not added yet

## Practical takeaway

If someone wants the most complete parity examples first, start with:

1. `multi-machine-interval-scheduling`
2. `knapsack-and-greedy-algorithms`
3. `transportation-and-transshipment-models`
4. `truck-cubing-bin-packing`
5. `network-capacity-transport-planner` for a more applied real-world planning shape
