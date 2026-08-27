# Style Block — Paste-Ready Generation Constants

**Status:** DRAFT v1 (2026-08-28) — derives from `01_narrative/craft-rules.md`
(LOCKED v1) + `02_dna/crowd-and-venue.md` (LOCKED v1, R1–R5).
**Purpose:** the single paste-source for every generation prompt. Everything
here is copy-paste; nothing here is paraphrased. If a constant isn't in this
file, it isn't a constant.

---

## 1. The anti-drift lead (first line of EVERY prompt)

```
Vertical 9:16 portrait video, thoroughbred horse racing
```

## 2. The style anchor (verbatim from craft-rules.md — never edited)

```
35mm lens, high shutter speed sports photography, broadcast 4K, photorealistic
```

## 3. The character blocks (paste from character-sheets.md, verbatim)

One block per character in frame, from `02_dna/character-sheets.md`.
Paste identical; never blend registers in one scene (yard blocks for yard
scenes, race-day blocks for race-day scenes).

## 4. Scene-type paragraphs (paste from crowd-and-venue.md §1)

For crowd-and-moment scenes (mounting yard, birdcage post-race, winning
post), paste the scene-type paragraph from `crowd-and-venue.md` §1. For built
locations, paste the canonical paragraph from `location-locks.md`.

## 5. The negative-prompt block (appends to EVERY prompt)

**Single paste-source: `crowd-and-venue.md` §11.** This file links it; it
does not copy it — a duplicate here would drift the first time one file
changes. Append the §11 block verbatim after the style anchor.
Wet-track variant (R3): relax `no rain, no fog`, permit mud; `no dirt track`
and all dress/betting bans stand.

## 6. Format constants

- 1080 × 1920 (9:16), 30/60 FPS.
- Text overlays in post only — never in the generation prompt.
- Center safe zone for overlays (clear of TikTok UI + bottom captions).
- NZTR regulatory micro-badge in brand gold `#d4a964`, subtle, safe zone.

## 7. Audio constants (from craft-rules.md, unchanged)

- 3-track mix: VO 0dB / SFX -10 to -14dB / music -18 to -22dB.
- Audio Snap: announcer 0–3s at +2dB→0dB; hard cut to silence 0.2s at 3.0s;
  intimate VO 0dB + yard SFX -12dB + music -22dB from 3.2s.
- VO register: Private Banker Standard — visual register is relaxed
  Australasian; the contrast is the signature. Layers never merge.

## 8. The quality-gate tests (apply to every generated frame)

- **Dress test (R5 canonical):** *"One notch above the pub — a notch below
  the Cup. Everyone made an effort; nobody was checked at the door."*
- **Two-viewer test:** NZ viewer: "that's here." Oz viewer: "same same."
  Nobody thinks England, Hong Kong, or Dubai.
- **Form test:** no frame confusable with betting or tipping; the horse's
  living shape is the reading.
- **Access test:** no frame implies exclusion at the rail.
- **Hero test:** the Thoroughbred is never outranked by any human or
  interface in frame.

## 9. Wet-track variant (R3)

- Sanctioned: genuine mud on grass — splash on legs/silks, choppy turf,
  light drizzle.
- Relax in negative block: `no rain`, `no fog`.
- Unchanged: `no dirt track`, all dress and betting bans.
- Still parked: night racing (no frame may be confusable with a night
  scene), full wet-day campaign variants (later).

## 10. One-line register summary (the signature in one sentence)

Relaxed Australasian people and places, Private Banker voice, golden-hour
and summer-sun turf, subject-sharp / world-soft, inside the rail — the
feeling is the product, and every surface ends on **"Own the Experience."**

---

*Derives, never defines. Constants express craft-rules.md under
crowd-and-venue rulings; they do not redefine either.*