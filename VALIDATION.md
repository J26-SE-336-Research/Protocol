# Validation

Validated with Go 1.23.12 on Linux.

- `go test -race -cover ./...`: passed.
- `go vet ./...`: passed.
- All Go source files formatted with gofmt.

Tests cover scalar syntax, core round trips, duplicate/missing headers, ranges,
response correlation and flags, deadline arithmetic, concurrent token spending,
child allocations, retry gates, topology truncation/conflicts and HTTP cloning.

This is reference-library validation, not distributed runtime conformance or
proof of research novelty. Run the same checks on your Mac after integration.
