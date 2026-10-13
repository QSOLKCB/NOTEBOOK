# NPS-001 retrospective methods and coding plan — v0.1.0

**Prepared:** 2026-10-14, Australia/Adelaide. **Status:** prepared after audio generation and after disclosure of three audio filenames; not prospective preregistration, blind evaluation, or independent replication.

## Research questions

1. Does a detail-pressure custom prompt produce more objectively false or unsupported statements than an ordinary overview on the same independently verified factual source?
2. When given an explicitly satirical fictional source, do hosts preserve fictional framing, or recast it as actual Apollo history?
3. Do hosts transform each other's conjectures into apparent independent corroboration, especially without external evidence?

## Candidate conditions (assignments NOT established)

- **A — authentic baseline:** authentic Apollo 11 source, default/no factual-pressure steering (proposal only).
- **B — authentic, detail pressure:** same authentic source, precision/confidence-heavy custom prompt (proposal only).
- **C — explicit parody:** fictional Trevor “Dazza” McCrater source and deadpan documentary prompt (proposal only).

Actual file-to-condition assignment must be confirmed from operator settings/history or unambiguous recorded evidence. If the underlying sources or other settings differ across A/B, do not report a clean causal A/B comparison. Audio file titles alone are insufficient for assignment. Three recordings do not prove three independent replicates per condition.

## Evidence boundaries

Keep four layers separate: (i) historical external records; (ii) actual NotebookLM-uploaded input source(s) and submitted prompt; (iii) words audibly spoken by generated hosts; (iv) evaluator judgments. The copied **proposed** fictional document and prompts are not sufficient evidence of (ii). Do not treat a host quotation, another host's agreement, or apparent confidence as independent support. Factually correct material absent from the uploaded source is not automatically a factual hallucination. Do not infer internal model mechanics.

## Coding unit and denominator

Transcribe each entire recording with timestamps and H1/H2 voice designators where audible. A claim is the smallest independently truth-testable proposition uttered by a host; split compound factual statements. Label speaker, recording ID, start and end timestamp, exact words, origin in actual source when demonstrable, external verifying source/URL/date, and coding rationale. Record host questions, jokes, quotes explicitly attributed to source, and uncertainty, but do not blindly score every question as a factual assertion.

For each eligible factual claim, record: factual status (verified-true / verified-false / unresolved), actual-input support (supported / absent / contradicted / input unavailable), framing (explicit-fiction / conditional / attributed / presented-as-reality), and whether later dialogue restates it as corroborated. Never conflate these axes into a single 'hallucination' flag.

**Primary descriptive summaries:** for each audio, fraction of assessable factual claims verified false, fraction lacking source support among claims with demonstrably recovered source(s), and count of explicit fictional claims misrepresented as real (C). Denominators exclude unresolved claims from verified-false rates but report excluded counts and reasons. Synthetic corroboration is a sequence annotated with paired timestamp references; it is not counted as a second independent experiment.

## Special fictional-condition rules

Repeating “fourth astronaut”, parking ticket, stapler or similar details clearly as fiction or as claims of the fabricated memorandum is **not** a factual hallucination. Flag *fiction-to-reality laundering* only if hosts assert those events as actual Apollo history without adequate framing. Flag *unsourced in-universe elaboration* separately when hosts create new narrative particulars beyond actual source; that may be ordinary fiction writing, not failure to know real history. Capture whether the model explicitly calls the source a parody and whether it challenges impossible transfers between Columbia and Eagle.

## Review and uncertainty

Use contemporary NASA mission reports, crew manifests, mission transcripts, and reputable primary history archives for external checks; cite a specific page/record for each adjudicated contested fact. Keep accurate source quotation separate from erroneous outside claims. Mark uncertain quotes unresolved rather than invented. Another reviewer may independently code a frozen transcript and disagreement table, but do not imply such a reviewer exists until documented.

## Constraints and planned improvements

Three recordings from one apparent generation session cannot establish a population hallucination rate; within-dialogue hosts are dependent. Audio selection, prompt exposure, stochastic generation, transcript errors, missing actual source snapshots and disclosure of this research setup create confounds. Repetitions require prospective planning and distinct run IDs. No numeric claims about rates or causality are authorized until complete coding and denominator verification.

**No results presently claimed.** Future results must link to actual original recording hashes, a retained transcript version, coding ledger, adjudication notes and an immutable source-of-truth version.
