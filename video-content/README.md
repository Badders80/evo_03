# video-content

Scoped project home for Evolution Stables video content (successor to the
evo_01 `06_content-pipeline/tik_tok` narrative work).

## Governing brand SSOT (this layer derives, never defines)

- `evo_00/doc/IDENTITY.md` (LOCKED, ADR-007) — master storyline + triad cadence.
- `evo_00/doc/VOICE_AND_TONE_MANUAL.md` (LOCKED SSOT) — voice, vocabulary, CTAs.
- `evo_02/packages/brand_dna/src/identity.ts` / `voice.ts` — code mirrors.

Binding rules for all video narrative extracted here:

1. `priceNeverInStory` — price points never appear in the story (late-funnel overlays only).
2. `noBorrowedAuthority` — AI characters are fictional; hype voices (e.g. race
   announcer) are quoted characters, never brand voice.
3. `surfacesDeriveNeverDefine` — video content derives from IDENTITY.md; the
   TikTok channel overlay is "Sensory yard" per the Voice Manual §Channel adaptations.

## Phase 1 — Narrative Extraction (current scope ONLY)

Source of extraction: `evo_01/pipelines/studio/06_content-pipeline/tik_tok/`
(STORY_STUDIO_ARCHITECTURE.md, PROMPT_MATRIX.md, campaigns/01–04, README.md).

- Extract and distill the narrative work already paid for: characters,
  locations, props, pundit personas, narrative bottles, story structures,
  prompt formulas.
- Output is curated markdown only. Curation, not rewriting — keep the
  hooks and voice that worked.
- Nothing ambiguous is silently dropped; unfinished items are marked `DRAFT`.

## Explicitly out of scope

- No DNA assets, no generation code, no pipeline tooling in this repo yet.
- No technical production (video gen, audio, assembly) — story layer only.
- No build debt carried from the old surface.

## Folder plan (unlocks as phases complete)

- `01_narrative/` — **DONE (Phase 1 locked v1):** `characters.md` ·
  `world.md` · `story-structures.md` · `bottles-and-hooks.md` ·
  `craft-rules.md`. Extraction inventory + rulings archived in
  `EXTRACTION_INVENTORY.md`.
- DNA / locked assets land here only after the story layer is signed off.

## Brand doc map (single map, one place each)

| Doc | Canonical home |
|---|---|
| Identity (who we are) | `evo_00/doc/IDENTITY.md` |
| Voice & tone | `evo_00/doc/VOICE_AND_TONE_MANUAL.md` |
| About & audience (founder, pillars) | `evo_00/doc/ABOUT_AND_AUDIENCE.md` |
| Design system / tokens | `evo_00/doc/DESIGN_SYSTEM_AND_TOKENS.md` |
| Code mirrors | `evo_02/packages/brand_dna/` |
| Video narrative (derives) | this repo, `01_narrative/` |

`evo_01/_shared/dna/` retired 2026-08-27 (pointer stubs only).