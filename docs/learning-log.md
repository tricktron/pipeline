---

## 2026-02-19: 02-pod-injection

### Acceptance Test
- Entry: `pkg/pod/pod.go` (`Build()`)
- Verified: 3 tests cover CA cert volume/mount/env injection for enabled, disabled/unset, and user override behavior

### Architecture
No new components. A conditional block was added to existing `Build()` to inject CA cert artifacts.

### Functional Core
- None (inline in `Build()`)

### Unit Tests
- Acceptance tests served as unit tests; no separate unit tests needed

### Discoveries
None
