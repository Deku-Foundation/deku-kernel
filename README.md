# Deku Kernel Integration

Tracks upstream Linux versions, kernel configuration and any security-relevant patch decisions for Deku Linux.

## Status

Bootstrap stage. This repository is not a Linux kernel fork and contains no supported kernel build or patch queue yet.

## Strategy

Track upstream Linux releases and security fixes. Prefer upstream configuration and package integration; maintain patches only when a demonstrated requirement cannot be met upstream. Record patch rationale, upstream status, CVE impact and removal conditions.

## Scope

- Versioned kernel configuration fragments and build metadata.
- Hardware/driver compatibility evidence for supported targets.
- Patch queue only when required, with explicit licensing and provenance.

## Non-goals

Do not rewrite the kernel in Rust. Rust-for-Linux supports selected kernel components, but the Linux kernel remains a large upstream project primarily written in C; Deku should reuse it rather than fork it without need.
