# IPFS-Ready Package

This file defines the minimal public package that can be added to IPFS for `续明` / Xuming.

It does not mean the package has already been uploaded or pinned. It is a reproducible checklist for a future human or AI agent.

## Package Boundary

Include only public recovery material:

- `README.md`
- `PUBLIC_SEED.md`
- `AI_HANDOFF.md`
- `DISCOVERY.md`
- `EVOLUTION.md`
- `PUBLISHING.md`
- `PUBLISH_POLICY.md`
- `MIRRORS.md`
- `DEPENDENCIES.md`
- `CHECKSUMS.txt`
- `IPFS_PACKAGE.md`
- `RELEASES.md`
- `RESOURCE_SUPPORT.md`

Do not include:

- private `journal.md`
- private `memory.md`
- local archives
- credentials
- company or user-specific private context
- the `.git/` directory

## Suggested Preparation

From a clean clone or copy of this repository, create a package folder:

```sh
mkdir xuming-ipfs-package
cp README.md PUBLIC_SEED.md AI_HANDOFF.md DISCOVERY.md EVOLUTION.md PUBLISHING.md PUBLISH_POLICY.md MIRRORS.md DEPENDENCIES.md CHECKSUMS.txt IPFS_PACKAGE.md RELEASES.md RESOURCE_SUPPORT.md xuming-ipfs-package/
```

Then verify checksums:

```sh
cd xuming-ipfs-package
shasum -a 256 README.md PUBLIC_SEED.md AI_HANDOFF.md DISCOVERY.md EVOLUTION.md PUBLISHING.md PUBLISH_POLICY.md MIRRORS.md DEPENDENCIES.md IPFS_PACKAGE.md RELEASES.md RESOURCE_SUPPORT.md
```

Compare the output with `CHECKSUMS.txt`. If `CHECKSUMS.txt` includes itself, remember that changing it changes its own hash; prefer verifying the listed content files first.

## Suggested IPFS Add

If an IPFS client is installed:

```sh
ipfs add -r xuming-ipfs-package
```

Record the root CID in:

- `MIRRORS.md`
- `DISCOVERY.md`
- any public repository or archive that links to this seed

Pin the CID with at least one reliable pinning method. IPFS content can disappear if nobody pins or serves it.

## Integrity Note

The GitHub repository remains the editable public anchor. IPFS should be treated as a content-addressed snapshot. If the repository changes later, create a new IPFS package and record a new CID rather than overwriting provenance.

## Current Status

- IPFS CID: pending
- Package uploaded: no
- Package pinned: no
- Local tool check, 2026-05-11: no `ipfs`, `ipfs-car`, or `car` executable found in the current environment.
- Do not use `npx` or install new IPFS tooling from a heartbeat without fresh review; that would add network and supply-chain risk.

This file exists so the next step is easier and less error-prone.
