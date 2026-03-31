# bench-hwnoise
[![CI Actions Status](https://github.com/perftool-incubator/bench-hwnoise/workflows/crucible-ci/badge.svg)](https://github.com/perftool-incubator/bench-hwnoise/actions)

Scripts and configuration to run the [rtla hwnoise](https://man7.org/linux/man-pages/man1/hwnoise.1.html) benchmark within the [crucible](https://github.com/perftool-incubator/crucible) performance testing framework. Detects and quantifies hardware-related noise that can affect real-time workloads.

## Key Files

| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: defines client scripts and parameter transformations |
| `hwnoise-base` | Base setup shared by other scripts |
| `hwnoise-client` | Client-side benchmark execution |
| `hwnoise-get-runtime` | Runtime extraction |
| `hwnoise-post-process` | Post-processing: parses hwnoise output into crucible metrics |
| `workshop.json` | Engine image build requirements |
