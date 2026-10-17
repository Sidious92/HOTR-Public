# HOTR Public CI Runner

Public GitHub Actions configuration for the private tabletop RPG repository `Sidious92/Heroes-Of-The-Rim`.

This repository contains **no private game rules, category data or code**. CI checks out an explicitly selected private commit into a temporary runner workspace using a narrowly scoped read-only GitHub Actions secret, tests it, and discards the checkout.

**Security:** never commit tokens or private source here; use GitHub Actions repository secrets. No private test logs, caches, artifacts or compiled catalogue exports should be published.

Workflow: `.github/workflows/hotr-gear-private-ci.yml` (manual dispatch and optional runner-config pushes).
