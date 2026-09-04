# Bench-hwnoise

## Purpose
Scripts and configuration to run the rtla hwnoise benchmark within the crucible framework. Detects and quantifies hardware-related noise (SMIs, NMIs, etc.) that can affect real-time workloads.

## Language
- Bash for client execution scripts
- Python for post-processing (`hwnoise-post-process.py`)

## Key Files
| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: client scripts, parameter transformations |
| `multiplex.json` | Parameter validation rules, unit conversions, and presets for multiplex |
| `benchmark-metadata.json` | Machine-readable description and CDM-indexed source/type list (consumed by `crucible benchmarks list`) |
| `hwnoise-base` | Base setup shared by other scripts |
| `hwnoise-client` | Client-side benchmark execution |
| `hwnoise-get-runtime` | Extracts runtime from command-line options |
| `hwnoise-post-process.py` | Parses hwnoise output into crucible metrics |
| `workshop.json` | Engine image build requirements |

## Conventions
- Primary branch is `main`
- Standard Bash modelines and 4-space indentation
- Python code follows 4-space indentation with standard modelines
