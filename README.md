# entities-humanoid-rom

A Lean 4 library for humanoid range of motion that states each joint's limit as one kusudama region, with muscle and prismatic constraints.

## What it is for

A joint's reachable set is a region on a sphere rather than three independent angle ranges, so the library models it as a kusudama and proves the domain logic in Lean. Adapters read biomechanics recordings and body-model sweeps into those limits and emit the constraint as shader source. `FINDINGS.md` records what its measurements found.

## Build

```sh
lake build
```

## Licence

MIT; see `LICENSE`.
