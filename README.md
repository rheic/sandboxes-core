# sandboxes-core

<img src="docs/assets/rheic-shark.png" alt="Rheic shark logo" width="180">


## Import path migration

The canonical Go module path is now `github.com/rheic/sandboxes-core` (previously `github.com/quoiner/sandboxes-core`). Update imports and `go.mod` requirements when moving to a release that includes this change. The old module path is not kept as a compatibility alias.

Status: pre-alpha.

Domain model, state machines, operation journal contracts, workspace rules, and
ports implemented by infrastructure modules.

## Boundaries

- no SQLite, containerd, HTTP, or os/exec;
- no dependency on runtime, gateway, daemon, or SDK;
- domain invariants live here and are enforced by the daemon.
