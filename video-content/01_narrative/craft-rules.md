# Craft Rules — Production Discipline (Reference Layer)

**Status:** LOCKED v1 (Phase 1 extraction)
**Scope:** How prompts and reels are built. This is discipline, not narrative —
it exists so the same story can't come out two different ways.

---

## The First Rule of Fight Club (price)

> We don't talk about the price. **We are selling the feeling** — the
> enjoyment, the human/animal relationship. The nominal purchase price never
> appears in narrative content: not in VO, not on screen, not in captions,
> not as "as low as $X". (Founder ruling 2026-08-27.)

- Never: "$85", "buy now for as low as", dollar figures, yield/return talk.
- Permitted only at the model level, late-funnel, outside the story:
  neutral phrases like "fixed price" — never a number attached to a story beat.
- Price surfaces only in late-funnel overlays (marketplace listing, campaign
  detail), per IDENTITY.md §4.1.

## Sensory Yard (channel register — Voice Manual §7.4)

- Angle: unpolished behind-the-scenes. Tone: raw, immersive.
- Video-first; short voiceover; natural stable sound leads.
- The platform is the quiet rail — never the hero. Handles are emotion,
  speed, shared joy, VIP access. The horse and the yard are the hero.
- Text/audio overlay carries ease and transparency — never price.

## Prompt engineering rules

1. **5-element formula** (see story-structures.md): camera + subject/action +
   setting + quiet-rail overlay + style anchor.
2. **Identical style anchor string everywhere:**
   `35mm lens, high shutter speed sports photography, broadcast 4K, photorealistic`
3. **<60 words per prompt.** Physical descriptors only.
4. **No text rendering in generation prompts.** Models mangle type — all
   text overlays go in post (Remotion/CapCut).
5. **Anti-drift lock:** lead with `Vertical 9:16 portrait video` + explicit
   `thoroughbred horse racing` to prevent 16:9 defaults and wrong-sport
   hallucinations.
6. **One-paragraph location lock** (from external reference method): the
   canonical location paragraph from `world.md` is pasted identical into
   every prompt using that location. The room stops drifting.

## Format & safe zones

- 1080 × 1920 (9:16), 30/60 FPS.
- Text overlays within the center safe zone (avoid TikTok UI + bottom captions).
- NZTR regulatory micro-badge in brand gold `#d4a964`, subtle, safe zone.

## Audio layering (3-track)

| Track | Content | Level |
|---|---|---|
| 1 | Master voiceover (Private Banker tone) | 0dB |
| 2 | Sensory SFX (hooves, gates, yard morning) | -10 to -14dB |
| 3 | Music (low-BPM) | -18 to -22dB |

Audio Snap mix: announcer 0–3s at +2dB→0dB; hard cut to silence 0.2s at 3.0s;
intimate VO 0dB + yard SFX -12dB + music -22dB from 3.2s.

## Brand compliance checks (pre-publish)

- No exclamation marks (unless verbatim quote).
- British English. No banned vocabulary (Voice Manual §2.3).
- One brand line max per asset; close on "Own the Experience."
- Fictional-quote flag present wherever a character speaks.
- Zero price talk anywhere in the story.