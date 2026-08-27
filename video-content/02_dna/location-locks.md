# Location Locks — Canonical Prompt Paragraphs

**Status:** DRAFT v1 (2026-08-28) — derives from `01_narrative/world.md`
(LOCKED v1) re-grounded under `02_dna/crowd-and-venue.md` (LOCKED v1, R1–R5).
**Purpose:** craft-rules rule 6 — the canonical location paragraph is pasted
**identical** into every prompt using that location. The room stops drifting.
**Re-grounding law (sanctioned Phase 2 job):** world.md's venue-agnostic
locations stay locked as narrative anchors; this file gives each one its
generation-ready paragraph — provincial NZ default, with venue-class mods
that ADD or SWAP texture without changing the emotional job.
**Venue law:** track and town names NEVER enter a paragraph (scene-type
locks, R-rulings 2026-08-28). Location IDs keep their historical names;
paragraphs stay placeless.

---

## `loc_dawn_yard` (re-grounds `loc_cambridge_dawn`)

**Canonical paragraph (provincial NZ default):**

```
Riverside training track at golden-hour dawn, low mist hanging off the green
turf rail, long shadows from a line of poplars, rolling green hills beyond
the running rail, dew on the grass, quiet apart from hoofbeats.
```

**Emotional job:** awakening, raw power, the ritual before the world wakes.
**Venue-class mods:** `metro_nz` — swap hills for tree-lined outer suburbs;
`oz_familiar` — wider flat horizon, more heat haze, drier-looking paddocks.
**Banned drift:** no stable complexes, no city skylines, no fog dense enough
to hide the horse, no rain (R3 wet variant excepted — light drizzle ok).

## `loc_parade_ring`

**Canonical paragraph (provincial NZ default):**

```
Grass parade ring enclosed by a white-painted rail, neatly mown lawn, a small
silver judge's box above, modest grandstand and summer crowd soft in the
background, bright midday sun, hard clean shadows across the turf.
```

**Emotional job:** heritage ceremony; the restricted-inner-circle moment —
earned, not gated (camera inside the rail).
**Venue-class mods:** `metro_nz` — larger grandstand, rose garden bed by the
gate; `oz_familiar` — wider ring, more heat shimmer, bigger distant crowd.
**Banned drift:** no dirt/sand rings, no herringbone raked European
enclosures, no corporate branding on rails, no Cup-scale fashion crowds.

## `loc_stables`

**Canonical paragraph (provincial NZ default):**

```
Timber stable block with raked barn walkway, early sunbeams cutting through
haze, brass latches, polished halter hooks, fresh straw, water bucket catching
the light, the yard dog asleep by the door.
```

**Emotional job:** intimacy and trust between owner and trainer — morning
access, the room where educated investment happens.
**Venue-class mods:** none needed — the yard is the same everywhere; only
light shifts (`oz_familiar` harder, whiter sun).
**Banned drift:** no clinical veterinary facility look, no American barn
red, no luxury-hotel stabling, no brand signage.

## `loc_owners_box` (re-grounds `loc_owners_lounge` — R4)

**Canonical paragraph (provincial NZ default):**

```
Light-filled trackside owners room with an open balcony onto the home
straight, timber floor, simple comfortable furniture, plants and framed
racing prints, coffee on the table, mid-afternoon sun streaming in, room
for a small group to stand together at the rail.
```

**Emotional job:** the owner's home base — shared joy with friends and
family. Ruled R4: modern sports-bar / casual-restaurant comfort, open and
sunny, **never dark and pokey**.
**Venue-class mods:** `metro_nz` — longer glass frontage, more seating;
`oz_familiar` — ceiling fans, deeper balcony shade on the edges only.
**Banned drift:** no walnut-panelled private club (retired with world.md
"mid-century walnut"), no dim lighting, no velvet-and-crystal opulence,
no screens showing odds or markets (form law) — TV in frame shows the
racing only.

---

## Scene-type cross-reference

The remaining v1 scenes (`scene_mounting_yard`, `scene_birdcage_post_race`,
`scene_winning_post`) take their canonical paragraphs directly from
`crowd-and-venue.md` §1 — they are crowd-and-moment scenes, not built
locations; the venue-class mods above apply to their backgrounds.

## Drift control

- One paragraph per location, verbatim, every prompt — no paraphrase, no
  "similar to".
- Venue-class mods are the ONLY sanctioned variation; they never change
  furniture, mood, or the emotional job — only scale, light, and horizon.
- The negative-prompt block (`crowd-and-venue.md` §11) appends to every
  location-bearing prompt.

| # | Item | Status |
|---|---|---|
| 1 | R4 re-ground of owners lounge (open, sunny, sports-bar/casual-restaurant) | Ruled 2026-08-28 — applied |
| 2 | "Mid-century walnut" retired from world.md's paragraph (world.md ID + emotional job unchanged) | Sanctioned Phase 2 re-grounding — veto if unwanted |
| 3 | Yard dog in loc_stables | Texture proposal — veto if unwanted |

*Derives, never defines. Paragraphs express locked locations under
crowd-and-venue rulings; they do not redefine world.md.*