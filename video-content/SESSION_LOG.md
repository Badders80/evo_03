# Session Log — 2026-08-27

## What was done

### 1. Phase 1 — Narrative extraction (DONE, locked v1, pushed)

- Created `evo_03/video-content/` as the scoped home for the video story layer
  (successor to `evo_01/pipelines/studio/06_content-pipeline/tik_tok`).
- Extracted + curated the old build's narrative into `01_narrative/` (5 files:
  characters, world, story-structures, bottles-and-hooks, craft-rules).
- Every file cites governing SSOT and carries derives-never-defines headers.
- Extraction inventory with verdicts archived in `EXTRACTION_INVENTORY.md`.

### 2. Founder rulings (applied, archived in EXTRACTION_INVENTORY.md)

1. Pundit personas (Liam/Arthur) DROPPED — design fresh later, nothing inherited.
2. Fight Club price rule — never the nominal price in the story; "fixed price"
   model-level only; $85 stripped from on-screen props.
3. "Own the asset." → "Own the Experience." (locked anchor).
4. Fictional colleague "Alex" renamed (no real-person implication).

### 3. Brand alignment fix (one-time full pass)

- Discovered the underlying DNA was already clean — the drift was in the old
  tik_tok consumer files, not the DNA.
- New canonical doc: `evo_00/doc/ABOUT_AND_AUDIENCE.md` (LOCKED SSOT) — migrated
  verbatim from `_shared/dna/about.md` (founder bio, audience, pillars, POV,
  origin, partnership guardrails). Commit `e184ee0`, pushed.
- Retired `evo_01/_shared/dna/` (4 files → MOVED-pointer stubs); re-pointed all
  live references: 04_comms AGENTS law, strategy/README, 3× AGENTS.md,
  evo_01 README, BRAND_KIT.md (caught by audit run 1, C14).

### 4. Kimi audits (3 runs, graph in audit-graph-2026-08-27.json)

- Run 1: 17/17 PASS — verified Phase 1 + brand migration claims (fixed BRAND_KIT.md live pointer mid-audit).
- Run 2: legacy submodule diagnosis — parent gitlink `f2e29aec` unreachable;
  content NEVER versioned (sprint-2 deleted legacy/.git, 244MB, during cleanup);
  `legacy/templates/` is LIVE (investor-update masters used 2026-08-21 send).
- Run 3: 04_comms dead-path repoint — 7 scripts fixed, 9/9 checks PASS.

### 5. Debt cleared

- `pipelines/studio/legacy` de-submoduled (commit `55e4757`): broken gitlink
  removed; 169 live/lightweight files tracked (incl. templates/); heavy dirs
  (poster-builder 86MB, racing_bot 71MB, gemini 17MB, out 38MB) gitignored,
  kept on disk pending founder keep/kill.
- 04_comms scripts: 7 files repointed from dead `/home/evo/evo_01` +
  `03_studio` paths to script-relative + `pipelines/studio/legacy/templates/`
  (commit `f1f901c` in submodule, pointer bump `a719adb` in parent).

### 6. Pushed

- evo_00 → GitHub (rebased over remote's build-loop commit; stash conflict in
  AGENTS.md resolved: Build Loop v1.1.0 + Git discipline both kept as laws 5+6).
- evo_03 → GitHub. 04_comms submodule → GitHub.
- evo_01 parent: NO remote (umbrella of nested repos — founder decision, do not fiddle).

## Open items (Phase 2)

1. **Venue/crowd DNA** — founder flagged: the 4 world locations are
   venue-agnostic; no dress code, crowd composition, or city-vs-rural texture
   anywhere in the build. Race records show our horses run at Tauranga (×3),
   Te Rapa (×3), Trentham, Wanganui. Strategic frame: story spans smallest
   track to Happy Valley/Meydan, but start NZ-targeted without alienating the
   industry. Proposed: `02_dna/crowd-and-venue.md` as first Phase 2 file.
2. Phase 2 file set: crowd-and-venue, character-sheets, location-locks,
   style-block, bottle-templates (one per bottle).
3. Separate small item: `pipelines/studio/legacy` continue.md has pending
   Track C purge + Remotion keep/kill decision (founder, not urgent).