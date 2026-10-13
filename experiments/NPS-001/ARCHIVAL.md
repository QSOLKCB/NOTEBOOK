# NPS-001 — Evidence completion and release checklist

## Already done on 2026-10-14

- Recorded three original user-provided M4A filenames, byte counts, local media properties and SHA-256 values.
- Prepared retrospective protocol and **unverified conversation-proposed** source/prompt references.
- Preserved unknown condition mapping rather than guessing from filenames.
- Opened a GitHub review branch with text-only metadata; **no audio was uploaded to GitHub**.

## Required before a full research claim or release

1. Retain **original** actual NotebookLM-uploaded source(s), source URL snapshots and exact custom instructions. Distinguish them from proposed examples above.
2. Enter authenticated condition ID (A/B/C or other) for each audio, exact generation settings, source count and generation time where genuinely known. Record unknowns without guessing.
3. Store unchanged M4A files in an immutable, versioned archive. Record precise per-file URLs, licence, bytes and SHA-256. A user-attached audio file is not automatically a permanent GitHub or Zenodo deposit.
4. Make full raw transcripts with timestamps and stable H1/H2 designators. Keep corrected transcripts separately; record the transcription approach and its errors.
5. Use the claim coding table and verify factual points against primary historical records. Re-review all contested claims.
6. Compute full denominators, uncertainty/limitations and descriptive outcomes. Do **not** assume that shared cues or host agreement are independent proof.
7. Package signed-off methods, metadata, artifacts, transcripts, claim ledger, results and fresh SHA256SUMS into the final archive. Only then update links to a specific Zenodo **version DOI** and an immutable repository commit.

## Rechecking the three original M4As

Place each of the original downloaded files beside `SHA256SUMS-audio.txt` and run:

```sh
sha256sum -c SHA256SUMS-audio.txt
```

A passing checksum establishes byte match to this recorded intake, **not** provenance of the original NotebookLM inputs, interpretation, publication or remote attestation.
