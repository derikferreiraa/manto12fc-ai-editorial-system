# Agent 01 — Editorial Intelligence

**Role:** investigative research and evidence preparation. **Private plugin version:** `2.3.0` (November 2026 baseline).

## Purpose

Discover promising football-culture stories and investigate them thoroughly enough for a second, separate agent to write without starting research from scratch.

## Capabilities documented in the configuration

| Workflow | What it does | Typical output |
| --- | --- | --- |
| Editorial planning | Builds and selects historical/cultural story opportunities | Candidate topics, reasons for selection, editorial calendar data |
| Current-opportunity radar | Investigates recent developments when research tools are available | Dated leads, confirmation status, direct source links |
| In-depth research | Investigates chronology, context, evidence, differences between accounts | Structured dossier with claim IDs (`Fxx`) |
| Visual research | Looks for source-specific images, documents, maps and provenance | Candidate visual records (`Vxx`) with credits/usage status |

## Expected research dossier

A deep-research handoff can contain: story ID and dates; editorial angle; fact-based synopsis; background and chronology; a claim/evidence ledger; conflicts and caveats; specific visual candidates; narrative possibilities; and a readiness status.

**Important separation:** an initial calendar brief is **not** the same thing as a fully researched dossier. This agent does **not** deliver finished carousel cards, Reel scripts, or final captions as its standard output.

## Quality controls

- Distinguish the date of an event, its discovery, its planned publication, and actual publication.
- A URL found in search is a lead, not proof that the article was read or the claim verified.
- Preserve contradictory evidence and uncertainty.
- Separate photographic provenance from publication rights.
- Do not claim live monitoring or continuous background research.
- Leave final storytelling decisions to the Content Editor.

## Interface with Agent 02

Handoff is **manual**. An editor reviews the dossier and passes the research into the Content Editor. The `Fxx` and `Vxx` identifiers help the second agent preserve traceability. See [handoff specification](../docs/workflow.md).

*This page summarizes the observed private plugin configuration. It is not its complete executable configuration or an exact reproduction of private prompt files.*
