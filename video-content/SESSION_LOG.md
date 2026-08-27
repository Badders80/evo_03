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

---

# Session Log — 2026-08-28

## What was done

### 1. Phase 2 opened — crowd-and-venue DNA LOCKED v1 (commit `282cf5b`, pushed)

- `02_dna/crowd-and-venue.md` built from founder rulings and **LOCKED v1**
  (audit run 4: 10 PASS / 1 WARN; WARN = Phase-1 conflicts routed to rulings,
  not silently edited).
- **Founder rulings R1–R5, all closed 2026-08-28:**
  - **R1** — 60/40 male/female featured-cast default; per-campaign flex
    (e.g. women's-day-at-the-races runs female-forward); lads block-buy =
    one recurring belonging beat, never the face.
  - **R2** — Jack's Barbour/tweed retired: yard = fashionable-cut oilskin
    vest over checked shirt (Rodd & Gunn-adjacent, INTERNAL calibration
    only — brand name never in a prompt, never on screen); trackside =
    shirt-tie-sunglasses, sports jacket, chinos.
  - **R3** — grass always; genuine mud permitted as wet-track texture (mud
    sits ON grass; `no dirt track` stands). Applied to locked
    `01_narrative/bottles-and-hooks.md`: dirt-splattered → turf-splattered
    (×3).
  - **R4** — owners box re-ground: "clean, functional, comfortable" =
    modern sports-bar / casual-restaurant feel, open and sunny, never dark
    and pokey; "mid-century walnut" retired.
  - **R5** — canonical dress test confirmed verbatim: *"One notch above the
    pub — a notch below the Cup."* Internal quality gate only.
- Form ruling (founder, earlier in session): we are NOT form analysis and
  NOT tipping — we show the horse's living shape (coat, stride, condition,
  warmup) at the source; betting is a derivative. §8 visual law encodes it.

### 2. Phase 2 file set DRAFTED (4 files + 4 templates, all DRAFT v1)

- `02_dna/character-sheets.md` — paste-ready blocks ×4. R2 applied to Jack;
  Emma linen summer default; silhouette test per character.
- `02_dna/location-locks.md` — 4 canonical paragraphs (dawn yard, parade
  ring, stables, owners box); venue-class mods change scale/light only;
  track names placeless.
- `02_dna/style-block.md` — anti-drift lead, verbatim anchor, negative-block
  single-sourced to crowd-and-venue §11, 5 quality-gate tests, wet variant.
- `02_dna/bottle-templates/` — 4/4 (Unlatched Chain, Morning Briefing,
  Meeting Snap-Back, Jockey High-Five): fill-in-the-blanks frame + Audio
  Snap beat map + locked VO verbatim + "Own the Experience." close +
  fictional-flag rule.

### 3. Audits (audit-graph-2026-08-27.json)

- Run 4 — crowd-and-venue draft: 10 PASS / 1 WARN (conflicts flagged, not
  silent).
- Run 5 — Phase 2 build-out: 8/8 PASS (anchor byte-match, VO verbatim,
  no-price grep clean, banned-register descriptors live only as "retired"
  doc lines).

## Open items (next session opens here)

1. **Founder sign-off on 4 flagged items** (silence-approves proposal on
   the table): (1) Emma linen summer register · (2) Tyler strap clipped
   once mounted · (3) Nellie braids race-day-only · (4) yard dog in
   stables paragraph. On sign-off (or veto): flip 4 drafts to LOCKED v1,
   commit + push as one unit.
2. Then: assemble one real test prompt per bottle from the DNA to prove
   the paste-chain end-to-end.
3. Candidate: feed R1–R5 rulings to gbrain hub as decision cards (evo_00
   AGENTS.md law) once Phase 2 fully locks.
4. Standing: legacy continue.md Track C purge + Remotion keep/kill
   (founder, not urgent).