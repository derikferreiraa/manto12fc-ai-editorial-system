<h1 align="center">Manto12FC — AI Editorial System</h1>
<p align="center"><strong>Two specialized AI agents. One human-directed editorial workflow.</strong></p>
<p align="center">Football culture · Editorial research · Content production · AI workflow design</p>
<p align="center"><a href="README.pt-BR.md">🇧🇷 Ler em português</a></p>

## Overview

**Manto12FC** is an independent football culture and storytelling project. This repository documents an **AI-assisted editorial workflow** designed to support its research and publishing process, from identifying a story and preparing researched copy and visuals to assembling the final graphic in an existing Canva template.

The system has **two separately configured ChatGPT plugins**, each responsible for a different part of the workflow:

| Component | Primary responsibility | Delivers |
| --- | --- | --- |
| **01 · Editorial Intelligence** | Identify, investigate, cross-check, and organize stories | Research dossiers, evidence logs, visual references, editorial caveats |
| **02 · Content Editor** | Transform research into an editorial narrative | Carousel copy, Reel/video scripts, captions, images or visual references where available |
| **Human design / Canva** | Place the selected content into Manto12FC templates | Final designed slides or static artwork for review |

> **Architecture note:** These agents **do not automatically communicate or execute one another**. A human selects the story, reviews the research, and manually passes the dossier from Agent 01 to Agent 02. The agents' **outputs are integrated through an intentionally designed handoff**, not a software API integration. After Agent 02, **the creator manually assembles the text and visual materials in a Canva template**; the plugins do not generate a finished Canva layout.

## Workflow

1. **Select a story.** Choose an angle, historical event, cultural connection, or relevant current development.
2. **Research with Editorial Intelligence.** Build a source-aware dossier, keeping facts, potential visuals, uncertainties, and dates separate.
3. **Review and transfer the dossier manually.** Use the documented handoff contract to preserve evidence and caveats.
4. **Produce with Content Editor.** Choose a narrative structure and develop the requested deliverable, with accompanying visual references where available.
5. **Design manually in Canva.** Select the texts and images or visual references from Agent 02, then place, crop, typeset, and adjust them in an existing Manto12FC Canva template. This layout step is performed by the creator, not automatically by either plugin.
6. **Review and publish.** Check claims, credits, usage rights, visual consistency, and the final artwork before publication.

### The research-to-production contract

The research plugin's handoff document distinguishes:

- `F01`, `F02`… — **factual claims**, their sources, verification status, and limitations.
- `V01`, `V02`… — **visual candidates**, what they depict, source, credit, and rights/usage status.
- **Editorial caveats** — disputed dates, conflicting versions, licensing questions, or facts requiring an update.
- **Readiness** — ready to draft, ready with caveats, or further research required.

This prevents the production stage from mistaking a plausible lead for a verified fact, or an image search result for a licensed asset. See [Handoff & architecture](docs/workflow.md).

## Specialized agents

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>01 / Editorial Intelligence</h3>
      <p><strong>Research before writing.</strong></p>
      <p>Historical planning, current-story discovery, in-depth research, and visual source investigation. Produces source-aware dossiers, but does not write final cards or scripts.</p>
      <p><a href="agents/01-editorial-intelligence.md">Explore Agent 01 →</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>02 / Content Editor</h3>
      <p><strong>Turn evidence into stories.</strong></p>
      <p>Develops captions, carousel copy, video/Reel scripts, and static-post content. Supplies images or visual references when available, proposes visual direction, and applies editorial validation. The creator then builds the artwork in Canva.</p>
      <p><a href="agents/02-content-editor.md">Explore Agent 02 →</a></p>
    </td>
  </tr>
</table>

## Design principles

- **Evidence before fluency.** Trace important claims to the researched source; preserve uncertainty.
- **Clear separation of work.** Research establishes what is supportable; production decides how to tell the story.
- **Human-in-the-loop.** Manual transfer, selection, Canva template assembly, fact review, and publishing approval remain human responsibilities.
- **Editorial consistency without templates.** The narrative format and number of slides depend on the story, not a fixed formula.
- **Visual provenance matters.** A compelling photo is not automatically authentic or licensed for reuse.
- **Reusable documentation.** The same process supports football history, identities, shirts, supporters, architecture, and current culture.

## From AI output to Canva artwork

The Content Editor provides publication-ready **copy** and, when available, **images, image previews, or source-linked visual references**. The Manto12FC creator then **manually places these elements into a Canva template**, adjusting typography, placement, cropping, and composition to produce the final visual publication. Previewed or suggested imagery is subject to attribution and usage-rights checks before incorporation. The system does **not** control Canva, automatically populate templates, or export the final designed artwork. See [manual Canva production](docs/canva-production.md).

## Repository guide

```text
manto12fc-ai-editorial-system/
├── README.md                  # English project overview
├── README.pt-BR.md            # Brazilian Portuguese overview
├── agents/
│   ├── 01-editorial-intelligence.md
│   └── 02-content-editor.md
├── docs/
│   ├── workflow.md           # Handoff specification and workflow
│   ├── canva-production.md   # Manual template design and final artwork
│   ├── quality-and-limits.md # Safeguards, scope, limitations
│   └── sources.md            # Documentation provenance
└── examples/
    └── handoff-scenario.md   # Illustrative scenario, not a live result
```

## Illustrative scenario

The [Arsenal/Gillespie Road handoff scenario](examples/handoff-scenario.md) demonstrates how a research topic can pass through the two-stage process. **It is an instructional example based on the plugin's acceptance-test topic, not a record of a completed production run or a historical fact-check.**

## Project status and technical scope

| Item | Status |
| --- | --- |
| Editorial Intelligence plugin | Documented from private version **2.3.0** |
| Content Editor plugin | Documented from private version **1.7.1** |
| Inter-plugin data exchange | **Manual and human-supervised** |
| Automatic orchestration / APIs | **Not implemented** |
| Automatic publishing / background monitoring | **Not implemented** |
| Canva template composition | **Manually performed by the creator** |
| Editorial approval | **Human responsibility** |
| Repository contents | **Public case-study documentation**, not deployable plugin source |

This is a **workflow-design and editorial-AI case study**, not a claim of autonomous execution or a turnkey application. The private plugin packages, editorial datasets, and third-party reference media are intentionally excluded.

## About

**Designed by Derik Ferreira** for Manto12FC, connecting communication, sports storytelling, editorial methodology, and applied AI.

[GitHub profile](https://github.com/derikferreiraa) · [Connect on LinkedIn](https://www.linkedin.com/in/derikferreira/)

*Documentation baseline: November 2026. All editorial outputs require review before publication. No third-party assets are redistributed in this repository.*
