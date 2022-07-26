# cypress-image-snapshot

## 4.2.1

- Updating peer dep to support versions of cypress beyond 4.5.

## 4.2.0

- Adding support to access details of snapshot diff failures even when using `failOnSnapshotDiff=false`. Details of diff failures can now be accessed from an object stored in `Cypress.env("snapshotDiffs")`, diff details are keyed by the name of the snapshot image.

## 4.1.0

- Using custom version of [jest-image-snapshot](https://github.com/thecapdan/jest-image-snapshot) and adding support for preserving newly created snapshots on failure.

## 4.0.1

### Patch Changes

- [`17f7927`](https://github.com/jaredpalmer/cypress-image-snapshot/commit/17f7927384bfdbd6cbb65d344c8337d32926b691) Thanks [@jaredpalmer](https://github.com/jaredpalmer)! - When using native retries that come in Cypress v5+ real image failures are marked as passed on the retries because cypress names the snapshots as 'filename (attempt X).png (and there is no configuration option to change this). The fix just removes the ' (attempt X)' suffix from the filename.
