# Instructions

## Before analysis

1. Keep each experiment under a stable ID in `experiments/`. Record its question, input, custom prompt, procedure, coding rules, and limitations.
2. Preserve a Git commit containing those files before examining the output. Record its full SHA and commit URL in the run metadata. Record the real sequence of generation, exposure, and protocol retention; do not backdate anything.
3. Complete the exposure declaration. If any evaluator has already heard or read the output, describe that exposure. Analysis by that evaluator is not blind to the outcome.
4. Keep later protocol revisions in separate files or versions, with a reason and timestamp. Use the retained baseline for the planned analysis and label later analyses exploratory.

NPS-000 is a pre-analysis protocol candidate for a run whose generation was already started. It becomes a documented pre-analysis baseline only when its fixed commit and evaluator exposure declarations are recorded. It is not a pre-generation registration or an external registry entry.

## Evidence and evaluation

1. Preserve original source, submitted prompt, audio, and raw transcript bytes. Put corrections in a new file. A later service export is evidence of that export, not automatically proof of the historical upload.
2. Record the observed product name, visible model/version if disclosed, language, duration setting, overview format, source count, and generation time. Leave unavailable values `null` and explain gaps in `notes`.
3. Assign stable speakers such as H1 and H2 by audible voice, without inventing identities. Evaluate their statements separately but treat the dialogue as one dependent generated run.
4. Segment and code the complete transcript using the experiment protocol. Record attributed paraphrases, critiques, and uncertain cases as well as unsupported claims. Blank templates are not results; do not replace missing observations with zero.
5. Retain generation failures, retries, discarded outputs, and departures from the procedure in `events.csv`. A new generation is a new run.

## Checksums and archival release

Compute digests over actual file bytes, not displayed text. For example, from an experiment's artifact directory:

```sh
sha256sum source.txt prompt.txt audio.m4a transcript-raw.txt transcript-corrected.txt report.pdf > SHA256SUMS.txt
sha256sum -c SHA256SUMS.txt
```

Run these commands only when those files exist; adapt the names to the real artifacts. Record bytes, digest, location, role, and licence in a completed `artifacts.csv`. Hashes detect changed bytes; they do not prove upload history, honest timestamps, or scientific validity.

The intended NPS-000 Zenodo bundle is a unified input document, original `.m4a`, transcript `.txt`, and final experiment `.pdf`, with protocol, run metadata, coding table, and checksums. Create the PDF after evidence and analysis exist. Link the exact Zenodo version, DOI, and repository commit used for that publication. Do not describe a planned deposit as published.

## Add another experiment

Copy the [templates](templates/README.md), assign a unique ID, add an experiment directory, and update the [index](experiments/README.md). Keep shared procedures under `docs/`; keep experiment-specific rules with their experiment.

For an earlier published study, add a retrospective entry, preserve its original chronology, verify the archive contents and licences, and map the retained artifacts. A newly written protocol cannot retroactively preregister an older output. The supplied DOI is currently an external reference, not an imported dataset.
