# Demuntu

Demuntu is the Ubuntu-based product layer for the local distro ISO factory.

This repository intentionally preserves the same relative paths used by the
`distro-packaging` build workspace:

```text
assets/boot/                  Demuntu boot and Plymouth source assets
configs/ubuntu/               Ubuntu desktop and server profile inputs
configs/spins/demuntu-*.toml  Demuntu spin declarations
packages/meta/demuntu-meta/   Demuntu branding and metapackage sources
docs/                         Product-relevant packaging notes
```

Build orchestration currently lives in:

```text
../distro
```

or any checkout of:

```text
https://github.com/PaulMDemers/distro-packaging.git
```

During active development, overlay this repo into the packaging workspace or
copy changed product files back into the same relative paths before running the
existing `make demuntu-*` targets.
