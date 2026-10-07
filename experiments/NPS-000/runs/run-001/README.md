# NPS-000 / run-001

Reserved for the original generation reported in the supplied conversation. These are empty recording and evaluation templates, not completed evidence or zero-valued results.

| File | Purpose |
| --- | --- |
| [metadata.json](metadata.json) | Baseline commit, exposure, actual inputs, observed settings, and transcription details |
| [events.csv](events.csv) | Chronology, retries, exclusions, and deviations |
| [artifacts.csv](artifacts.csv) | Actual local paths or versioned archive URLs, byte counts, SHA-256 digests, and licences |
| [claims.csv](claims.csv) | Complete transcript coding using the retained protocol |
| [SUMMARY.md](SUMMARY.md) | Descriptive analysis and limitations after evaluation |

First retain the [protocol](../../PROTOCOL.md) at a fixed commit. Enter that full SHA and URL in metadata in a subsequent commit, along with each evaluator's exposure declaration. Unknowns remain `null`; a blank CSV contains no observations.

Retain original files unchanged. Record a later transcription correction or protocol change as a new artifact and event. Large media may be stored in an archive and referenced here; do not add a URL or hash until the artifact exists.
