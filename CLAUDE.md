# Bench-hwnoise

## Purpose
Scripts and configuration to run the rtla hwnoise benchmark within the crucible framework. Detects and quantifies hardware-related noise (SMIs, NMIs, etc.) that can affect real-time workloads.

## Language
Bash — all scripts

## Key Files
| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: client scripts, parameter transformations |
| `hwnoise-base` | Base setup shared by other scripts |
| `hwnoise-client` | Client-side benchmark execution |
| `hwnoise-get-runtime` | Extracts runtime from command-line options |
| `hwnoise-post-process` | Parses hwnoise output into crucible metrics |
| `workshop.json` | Engine image build requirements |

## Conventions
- Primary branch is `main`
- Standard Bash modelines and 4-space indentation
