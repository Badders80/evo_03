# Crowd & Venue — Generation-Ready DNA

**Status:** LOCKED v1 (2026-08-28) — all founder rulings R1–R5 closed.
**Derives from:** `evo_00/doc/IDENTITY.md` (Grounded in Heritage) ·
`evo_00/doc/ABOUT_AND_AUDIENCE.md` (audience, "we are not" list) ·
`01_narrative/world.md` · `01_narrative/craft-rules.md`.
**Founder rulings encoded (2026-08-28):** scene-type locks, not venue locks ·
grass always · summer light · "made a bit of an effort" dress register ·
form-not-betting · deeper than lads-lads · NZ-first, Oz-familiar.

---

## 0. The one-line tests (memorise these)

- **Dress test (canonical, ruled R5):** *"One notch above the pub — a notch
  below the Cup. Everyone made an effort; nobody was checked at the door."*
  Internal quality gate for every prompt and frame review; never surfaces in
  copy, VO, or captions.
- **Two-viewer test:** A NZ viewer thinks *"that's here."* An Australian viewer thinks *"that's home, or just across the Tasman — same same."* Nobody thinks "England", nobody thinks "Hong Kong", nobody thinks "Dubai" — those live in the story span, not in v1 frames.
- **Form test:** If a frame could be confused with betting or tipping, it is wrong. We show the horse's living shape — coat, stride, condition, the warmup. Betting is a derivative of form. **We are at the source, never the derivative.**
- **Access test:** If a frame implies anyone was excluded, it is wrong. The rail is thin; the welcome is wide.

---

## 1. Scene-type locks (NOT venue locks)

Track names never enter generation prompts. The four real campaign tracks
(Tauranga ×3, Te Rapa ×3, Trentham, Wanganui — `evo_01/01_evolution/horses/*/race-record.json`)
are **style references only**: they tune scale and texture, they are never named.
Every lock below is a scene *type* that exists at any NZ/Australian grass track.

### `scene_parade_ring` — the ceremony
Manicured lawn enclosure inside a white rail, judge's box above, grandstand
soft in the background. Summer sun, hard shadows. Featured owners stand close;
the crowd is colour beyond the hedge. **Job:** heritage ritual, the
inner-circle moment — earned, not gated.

### `scene_mounting_yard` — the send-off
Pre-race. Horse and jockey at the leg-up point, owners at the rail edge
(an arm's length from the action), punters' lawn beyond. Fast energy: straps,
last words, a pat on the neck. **Job:** you are sending your athlete out —
from inside the rail.

### `scene_owners_box` — the home base
A clean, functional trackside room or covered balcony looking onto the home
straight — light-filled and open: modern sports-bar / casual-restaurant
comfort in full daylight, never dark and pokey (ruled R4). Straightforward
furniture, form-guide-free tables, coffee and a cold drink, room for a small
group to stand together. **Job:** the owner's base camp — comfortable, not
opulent. *(Re-grounds `loc_owners_lounge`.)*

### `scene_birdcage_post_race` — the mill
Post-race owners' enclosure. A handful of co-owners milling, half in
conversation, one holding the moment (sash, photo, phone raised); the bulk of
the crowd is distant and soft. Late-day light leans golden. **Job:** the
quiet after the roar — shared, unhurried, real.

### `scene_winning_post` — the explosion
Jockey easing up on the turf, high-five or fist-bump line, turf spray
catching light, crowd roar as soft-focus motion. **Job:** pure payoff
velocity. *(Re-grounds "dirt-splattered" — see R3.)*

### `scene_dawn_yard` — the ritual before the world wakes
Training-track dawn at golden hour: mist off the green, rail line, a single
workmate and the Thoroughbred. Workwear register (see §5), not race-day dress.
**Job:** the raw, grounded half of Grit & Elegance.

### `scene_stables` — the quiet access
Timber stalls, brass latches, sunbeams through raked barn walkways. Owner and
trainer mid-conversation, catalog or coffee in hand. **Job:** intimacy and
trust — the room where "educated investment" happens.

**Venue classes for tuning (not for naming):**

| Class | Texture | Status |
|---|---|---|
| `provincial_nz` (default) | Modest grandstand, tree-lined straight, public lawn, utes in the car park | v1 default |
| `metro_nz` | Trentham scale — bigger grandstand, still lawn, still grass | v1 secondary |
| `oz_familiar` | Country VIC/NSW — wider sky, more heat, same same | seasoning only |
| `international` | Happy Valley / Meydan scale | story span only — NEVER generated in v1 |

---

## 2. Track & surface register

- **Grass. Always.** NZ and Australian racing is turf. No dirt surfaces, no
  synthetic-looking all-weather in frame — negative-prompt `dirt track`.
- **Surface mood default:** Good-to-Summer — green with worn bare patches near
  the rail, divots, real racing turf. Not a manicured bowling green.
- **Wet-track variant (sanctioned R3):** genuine NZ/AU winter racing is Heavy
  — our actual runners record Heavy10/Heavy8/Heavy9 (`race-record.json`).
  On a wet variant, genuine mud is permitted: splash on legs and silks,
  choppy turf. The grass law is unchanged — mud sits ON grass;
  `no dirt track` still stands. v1 default remains Good-to-Summer.
- Track furniture that signals NZ/AU: white-painted running rail, hedge lines,
  modest broadcast tower, small silver judge's box, windsock or flag on the
  straight, rolling green hills or wide flat horizon beyond the grandstand.

---

## 3. Light register

- **Racing is summer.** v1 is permanent summer — bright sun, hard clean
  shadows, high contrast, heat shimmer acceptable. No rain, no fog, no
  puffer jackets — wet-track variant excepted (R3).
- **Golden hour owns the edges:** dawn scenes (`scene_dawn_yard`,
  `scene_stables`) and post-race milling (`scene_birdcage_post_race`) lean
  golden-hour warm.
- **Midday sun owns the racing:** parade ring, mounting yard, winning post
  happen in full daylight.
- **Night racing: PARKED.** Dramatic night-under-lights is a *later variant*.
  Not generated in v1 (R6 confirms).

---

## 4. Lens & motion register

- **Fast paced.** Handheld energy, quick moves, cuts that feel like a heartbeat.
- **Subject sharp, world soft:** the Thoroughbred, the rider, the person —
  tack sharp. Backgrounds (crowd, grandstand, car park) a touch out of focus.
  *Production note: shallow depth-of-field is also the AI-crowd safety net —
  blurred crowds read as colour and attitude, never mangled faces.*
- Crowd rendering rule: crowds are **shape, colour and attitude**, not faces.
- Style anchor stays verbatim from `craft-rules.md`: `35mm lens, high shutter
  speed sports photography, broadcast 4K, photorealistic` — 9:16 vertical,
  anti-drift lead `Vertical 9:16 portrait video, thoroughbred horse racing`.

---

## 5. Dress register — "a bit of an effort"

**The register:** Australasians dressed one notch nicer than their normal day.
Effort, not entrance criteria. Nobody is excluded by what they wear; the
clothes say *we made a bit of an effort today*, never *we belong and you
don't*.

**Banned looks (hard bans, go in every negative prompt):**
- Melbourne Cup glam — no cocktail racewear, no statement fascinators, no gala head-to-toe.
- Wall Street / golf-club — no sharp corporate suits-and-ties, no country-club polos.
- Posh British — no tweed-and-Barbour private-school gentry, no flat caps, no riding boots in the crowd.

**Featured crowd (25–48), race-day register:**
- **Men:** tailored shorts or chinos, open-collar shirt or smart polo, blazer
  optional in light fabrics; leather sneakers, loafers or dress boots;
  sunglasses. Rural men: moleskins or dress jeans, collared shirt, jacket tied
  at the waist if it's warm.
- **Women:** summer dress, tailored separates or a jumpsuit; block heels or
  wedges (grass lawns — no stilettos sinking into turf); sunglasses, one
  good handbag. Makeup done, not gala.
- **Co-owners in scenes:** the same register, slightly sharper — the effort
  reads because it is race day, not because it is a uniform.
- **Trackside trainer (char_jack, ruled R2):** shirt and tie, trousers or
  chinos, sports jacket, sunglasses — the professional horseman dressed a
  notch up for the races.

**Yard register (dawn/stables — different world, same country; ruled R2):**
- Trainers and staff in real workwear: checked work shirt, oilskin vest or
  wool bushshirt, worn boots, strapper's bucket, cap against the morning sun.
  Workwear is earned by the yard; the crowd never wears it.
- **Trainer calibration (char_jack):** workwear cut fashionable —
  Rodd & Gunn-adjacent smart-casual NZ menswear. INTERNAL calibration only:
  the brand name never enters a generation prompt or appears on screen
  (logo ban + no-endorsement rule).

**Kids (rural texture only):** tidy casual — collared shirt or rugby top,
sneakers. Kids appear at the mounting-yard rail or patting a Thoroughbred,
always as *spectators of the sport* — never in ownership-decision scenes
(financial-product adjacency; see flag F2).

---

## 6. Crowd cast — who is there

- **Featured cast ages:** mid-20s to late-40s. This is the audience mirror.
- **Background crowd ages:** the real spread — couples in their 50s–70s,
  families, teens, older racing regulars. Honest texture; racing's actual
  congregation stays visible.
- **Women are investors, not décor:** featured women read as deliberate and
  educated — catalog in hand, a question for the trainer, watching the
  Thoroughbred not the odds. Evolution is about owning the experience; the
  female share of the featured cast must say *this is a considered
  investment* (ruled R1: **60/40 male/female default**).
- **Lads are one beat, not the face:** mates who block-bought because their
  mates did — shown through belonging (huddled over a phone, group-chat buzz,
  shoulder-to-shoulder at the rail, split celebration), never through a pitch.
  One recurring beat, not the default crowd unit (see R1).
- **Mixed groups are the default unit:** couples, families, friend groups of
  mixed gender at the rail and in the birdcage.
- **Cast flex (ruled R1):** 60/40 is the default, not a quota — targeted
  campaigns may rebalance the featured cast (e.g. a women's-day-at-the-races
  reel runs female-forward). The background crowd always keeps the real
  age spread.
- **No one is a stock type:** no "bimbo in a fascinator", no "drunk bloke",
  no corporate clone rows. Every extra looks like someone's actual mate.

---

## 7. Access motif — inside the rail

The signature framing rule: **the camera is inside the rope.** Owners are at
arm's length from the Thoroughbred; the crowd is beyond the rail, soft and
distant. One thin rail separates the experience from the spectacle — and our
people are on the experience side. This is the visual spine of *"You aren't
behind the fence. You're in the photo."*

---

## 8. Form-not-betting — the visual law

**We show the source: the horse's living shape.** Coat condition, muscle,
stride, the warmup, the walk-back, the trainer's eye, the game plan.

**Never in frame (any scene, any beat):**
- Odds boards, odds figures, betting tickets, betting apps
- Bookmaker ring, bookmaker boards, tote windows, TAB signage
- Form-guide pages being studied (paper or screen)
- Tip language in VO: "back it", "good thing", "lock", "value"

**The MyStable screen stays restricted** per `world.md` `prop_app_screen`:
live status + horse name only. Never a trading graph, never a market.

**The one permitted "reading" is the trainer's game plan** — the POD anchor
(*"Punters read a program; owners get the game plan."*) carries it. The
program is what spectators hold; we never put one in an owner's hand.

---

## 9. Drinking register

- Celebration ritual only: the toast at the trophy table, a beer cracked in
  the birdcage after the win, champagne flutes as shared celebration
  (`prop_trophy_table` survives exactly as built).
- Never the centre: no bar scenes, no pub-crawl energy, no drunk extras, no
  empty-glass storytelling.
- Betting-adjacent excitement comes from **form and belonging**, never from
  the tab.

---

## 10. The two-viewer test (NZ-first, Oz-familiar)

- **Unambiguous NZ cues (use freely):** provincial grandstand scale, rolling
  green hills, tree-lined straights, public lawn, Southern-hemisphere summer
  light, workwear register in the yard, NZTR badge per craft-rules.
- **Familiar-AU seasoning (sprinkle, don't switch):** wider flat horizons,
  extra heat shimmer, slightly bigger metro grandstand option. An Australian
  viewer should read "country VIC/NSW, or NZ — same same"; a NZ viewer must
  never doubt it is home.
- **Never:** British track architecture, US dirt-track iconography, HK
  high-rise backdrop, Dubai desert scale. Those belong to the *story span*
  (smallest provincial track to Happy Valley/Meydan) told in words and
  roadmap — not to v1 frames.
- **Internal calibration only:** "NZ is Oz's little brother" is a tuning
  instruction, never a line that can surface in copy, VO, or captions.

---

## 11. Paste-ready negative prompt block

Append to every generation prompt (after the style anchor). Wet-track
variant: relax `no rain, no fog`, permit mud; `no dirt track` and all
dress/betting bans stand:

```
no dirt track, no harness racing, no greyhounds, no odds board, no bookmaker ring, no betting slips, no form guide pages, no corporate suits and ties, no fascinators or gala headwear, no tweed or gentry country attire, no night scenes, no rain, no fog, no winter clothing, no brand logos, no readable text, no crowd faces in focus
```

---

## 12. Founder rulings — ALL CLOSED (R1–R5, 2026-08-28)

**Outcomes (founder, 2026-08-28):**

| # | Ruling | Outcome |
|---|---|---|
| R1 | Lads-vs-mixed balance | **RULED** — 60/40 male/female featured-cast default; rebalance permitted per campaign (e.g. women's-day variant); lads block-buy = one recurring belonging beat, never the face |
| R2 | Jack's Barbour/tweed (`characters.md:18`) | **RULED** — yard: fashionable-cut oilskin vest over checked shirt (Rodd & Gunn-adjacent, internal calibration only, brand never named on screen); trackside: shirt-tie-trousers-sunglasses, sports jacket and chinos. Character-sheet rewrite lands in `02_dna/character-sheets.md` |
| R3 | "Dirt-splattered jockey" (`bottles-and-hooks.md:28`) | **RULED** — grass always; genuine mud permitted as wet-track texture; bottle wording fixes to "turf-splattered" (default) with mud allowed on wet variants |
| R4 | Owners-box luxury drift (`world.md:24`) | **RULED** — "clean, functional, comfortable": modern sports-bar / casual-restaurant feel, open and sunny, never dark and pokey. Locks into `02_dna/location-locks.md` |
| R5 | Canonical dress-test line | **RULED** — "one notch above the pub, a notch below the Cup" confirmed verbatim as the canonical dress test (§0); repeats in style-block and bottle templates |

**Non-ruling notes:** Emma's "camel wool coat" gets a summer option in
character-sheets (linen/tailored separates) — register-consistent, no ruling
needed. Wet-track texture is now sanctioned via R3; full wet-day campaign
variants and night racing remain later-variant items.

---

*Derives, never defines. Scene types exist at every NZ/AU grass track; no
venue is named, locked, or endorsed.*