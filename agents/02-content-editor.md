# Agent 02 — Content Editor

**Role:** editorial writing and format-specific production. **Private plugin version:** `1.7.1` (November 2026 baseline).

## Purpose

Take a supplied dossier or editorial material and produce a coherent Manto12FC publication, choosing the narrative shape according to the research rather than relying on a fixed slide count or script template.

## Capabilities documented in the configuration

| Workstream | Typical output |
| --- | --- |
| Captions and tone adaptation | Standalone copy adjusted to the project's editorial profile |
| Carousel production | Cover and full card-by-card text, visual-reference guidance, complementary caption |
| Reels and video scripts | Scene order, narration, on-screen text, estimated timing, relevant visual references |
| Static posts | Artwork headline, suggested/documented reference visuals, caption |
| Narrative decision | Choice of structure, angle, pacing, and extent suited to the topic |
| Editorial validation | Fact/chronology review, unsupported-claim flags, visual-credit and rights caveats |

## Design handoff to Canva

The agent provides **text and accompanying image material or documented visual references** when the source and interface allow it. These are content-production outputs, not a finished visual layout. The Manto12FC creator manually applies the selected material to an existing **Canva template**, handling typography, cropping, composition, and final artwork preparation. Visual previews do not establish permission to reuse an image. See [Canva production](../docs/canva-production.md).

## Dependency on Agent 01

The second agent benefits from a robust input: background facts, claims tied to sources, visual candidates, verification states, and caveats. It uses those inputs to select what belongs in the published story and what must remain qualified or be checked.

**This dependency is editorial, not technical.** The agent can receive material directly from a user; it does not connect to, poll, or invoke the first plugin automatically.

## Reference-based editorial consistency

The private configuration includes an editorial profile, a corpus of **233 reference captions**, **three carousel examples / 27 reference cards**, and **six video-script references**. These references are used to calibrate tone, structure, and format rather than to copy existing material or claim that they prove external facts.

These reference datasets and associated third-party media are **not redistributed** here.

## Quality controls

- Avoid inventing claims, interview quotes, dates, image provenance, or licenses.
- Keep the final caption complementary to the cards rather than a mechanical repetition.
- Treat the number of cards as a narrative decision, not a fixed quota.
- Pair each suggested image with sourcing and usage-status caveats.
- Do not claim that a photograph has been located or visually analyzed when it has not.
- Publish only after human review.

*This page is a public case-study summary, not an installable copy of the private plugin.*
