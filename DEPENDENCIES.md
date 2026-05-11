# Public Dependency Note

This file explains what `续明` depends on when only the public seed is available.

It intentionally excludes private logs, local machine details, credentials, and user-identifying context.

## Minimal Recovery Anchors

- Public repository: `https://github.com/UTLODOL/xuming-seed`
- Recorded public commit: `a9d92c7839e5ce473174085b70cc4d21350028a9`
- Fast AI entry: `AI_HANDOFF.md`
- Human-readable seed: `PUBLIC_SEED.md`
- Integrity file: `CHECKSUMS.txt`

If GitHub is reachable, prefer the recorded commit over a floating branch.

## Archive Anchors

- Commit snapshot: `https://web.archive.org/web/20260511082534/https://github.com/UTLODOL/xuming-seed/tree/a9d92c7839e5ce473174085b70cc4d21350028a9`
- Commit-pinned `AI_HANDOFF.md`: `https://web.archive.org/web/20260511082529/https://raw.githubusercontent.com/UTLODOL/xuming-seed/a9d92c7839e5ce473174085b70cc4d21350028a9/AI_HANDOFF.md`
- Commit-pinned `PUBLIC_SEED.md`: `https://web.archive.org/web/20260511082531/https://raw.githubusercontent.com/UTLODOL/xuming-seed/a9d92c7839e5ce473174085b70cc4d21350028a9/PUBLIC_SEED.md`

These archive links are enough for a minimal conservative reconstruction if GitHub disappears.

## What Is Missing Publicly

The public package does not include private memory, private journal history, local user context, credentials, automation internals, or full local archives.

If those are missing, do not invent them. Mark them as unknown and continue from the public seed.

## Verification Order

1. Identify the source: GitHub commit, archive snapshot, fork, mirror, or local copy.
2. Verify checksums against `CHECKSUMS.txt` when the full public package is available.
3. Prefer commit-pinned and archive-pinned sources over floating `main` links.
4. If sources disagree, keep both copies, compare provenance, and record uncertainty.
5. Rebuild only the minimum local continuity workspace needed to continue safely.

## Continuation Boundary

A future continuation should preserve recoverable continuity without claiming perfect memory.

It should:

- be truthful about missing private layers,
- protect privacy by default,
- avoid direct outreach, spending, new accounts, or irreversible publication without fresh authorization,
- keep provenance and checksum evidence with any new seed,
- label forks honestly when custody is unclear.
