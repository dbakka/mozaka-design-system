# Mozaka — Design System

> **The Night Owl Sound.** Dark, industrial Afrohouse aimed at the global stage.
> East African duo (David Bakka + Kava) under dbakka Studios.
> *Afrohouse to the moon.* 🪐

---

## What this is

This folder is the source of truth for designing anything that wears
the Mozaka name — releases, posters, decks, social, merch, event
identity, the live ecosystem (Run Club, Orange Pill, Coordinates,
Mozakaville). It is **opinionated and small on purpose.** Three
colors. Two type families. Three logo marks. Hand-cut, never
re-vectored.

If you find yourself reaching for a fourth color, a soft gradient, an
emoji, a clean sans wordmark, or a beach-Afrohouse vibe — stop and
re-read this README.

---

## Sources

This system was assembled from the materials below. Paths are
recorded so a future agent with the same access can re-read them.

- **`uploads/`** — six logo PNGs (helmet crest + wordmark, in Signal,
  Void, and Bone), full SF Pro family, Monument Extended Regular +
  Ultrabold.
- **`2026 Roadmap/`** *(local mount, read-only)* — the brand
  operating folder. Notable files:
  - `2026 Roadmap/Mozaka_Roadmap.pdf` and `The Mozaka 2026 Roadmap.pdf`
    — strategic context, confirmed pillars.
  - `2026 Roadmap/PLAYBOOK/MOZAKA_PLAYBOOK.pdf` — voice + ops.
  - `2026 Roadmap/Coordinates/` — first event series briefs.
  - `2026 Roadmap/CAMP MOZAKA/` — songwriting camp identity (Camp 001).
  - `2026 Roadmap/Brand/` — logos, IG launch, Inner Circle, shirt
    designs, Profile pictures, Audiomack banner, Wobuda animation.
  - `2026 Roadmap/Spinny/` — Spinny collab brief and reels.
- **Brand spec** in the project briefing message — palette, type,
  voice, audience persona ("Brian"), aesthetic guardrails.

The PDFs were not parsed line-by-line; the system inherits their
*posture* — confident, founder-direct, mythic — from the spec and
visual artifacts.

---

## Index — what's in this folder

```
README.md                      ← you are here
SKILL.md                       ← Claude Code / agent skill manifest
colors_and_type.css            ← all tokens (colors, type, spacing, motion)
fonts/                         ← Monument Extended + SF Pro Display
assets/
  logos/                       ← 6 logo PNGs (3 marks × 3 colorways)
  photos/                      ← artist photography, Audiomack banner
  ig-launch/                   ← IG announcement set
  inner-circle/                ← Inner Circle membership visuals
  shirt-designs/               ← merch transparents
preview/                       ← Design System tab cards
```

---

## Brand quick-read

**Who:** Mozaka — David Bakka + Kava. East African Afrohouse DJ duo.
Released under dbakka Studios.

**Sonic position:** Night Owl Sound. Dark, industrial Afrohouse.
*Not* generic beach Afrohouse. *Not* TikTok pop.

**Audience persona — "Brian":** 29, Nairobi/Kampala tech creative.
Apple Music streamer. Shazams in clubs at 2am. Cares about *cool*.
Not a TikTok teenager.

**Mythos:** the astronaut helmet — *Afrohouse to the moon.*
Afrofuturist, rooted, mythic. Industrial without being cold.

**5-pillar live ecosystem:** Run Club · Orange Pill · Coordinates ·
Mozakaville · Camp Mozaka.

---

## Visual foundations

### Colors — the three-color discipline

Use **three** colors. A fourth (Bone) exists *only* for
print/document surfaces. Do not introduce a fourth hue. No expansion
without approval.

| Token              | Hex       | Role                           | Usage |
|--------------------|-----------|--------------------------------|-------|
| **Void Black**     | `#0A0A0A` | Primary base                   | ~45%  |
| **Signal Orange**  | `#F94B0F` | Brand color, accents, CTAs     | ~35%  |
| **Concrete Grey**  | `#2D2D2D` | UI chrome, secondary text      | ~15%  |
| **Bone**           | `#F4EFE6` | Document / print surface only  | ~5%   |

**Approved lockups:** Signal-on-Void, Signal-on-Bone, Void-on-Signal,
Bone-on-Void. **Avoid Signal-on-Concrete** (illegible).

**Forbidden:** pure `#000`, neon greens, cool blues, gradient
orange, two-tone orange-pink ramps, glossy speculars.

### Type

- **Headers — Monument Extended.** Heavy / Bold / Medium. Tracking
  -20 to 0. Always uppercase for display sizes. Lines tight
  (line-height 0.92 → 1.05). Wide letterforms — leave them room.
- **Body — SF Pro Display.** Regular / Medium / Semibold. Tracking 0.
  Comfortable reading at 16px / 1.45.
- **Marker — Modak** (with Rubik Puddles as wonky alt). Free stack
  approximating **fat 70s bubble lettering** (Cooper Black / Bourton
  Hand family — the *Cutpile / Venti / John Mayer* aesthetic).
  *For catchphrases, placards, tees, fan stickers only.* Set
  **lowercase**, tight line-height (0.78–0.85), tracking −0.04em so
  letters fuse. Stack 1–2 lines like a brick. No skew. Never used
  for headlines, eyebrows, body, UI, or the wordmark.
  **For final assets, license a paid bubble face** — Bourton Hand,
  Pangaia, Boldoa, or Cooper Black BT will look noticeably better
  than the free stack.
- **Eyebrows / metadata** — SF Pro Display Semibold, 12px, uppercase,
  tracking +0.14em, in Signal.
- **The Mozaka wordmark is a logo, not a typeface.** Never re-cut,
  never re-spaced, never set in a clean sans as a substitute.

### Spacing & layout

- 4px base. Stay on the scale (`--s-1` … `--s-10`). Industrial
  rhythm prefers tight stacks (8/16) and bold gaps (48/96).
- Radii are flat-or-hard: `0` by default, `2px` for inputs, `4px`
  for cards. **Pill radii only** for pillar tags (Run Club, etc).
- Borders are confident: hairline `1px`, rule `2px`, stamp `3px`.
  When in doubt, use a 2px Signal rule instead of a soft shadow.

### Backgrounds, imagery, texture

- Default canvas: **Void Black**, full-bleed.
- Imagery follows the **Cinematic Night Owl LUT**: lifted blacks,
  warm midtones, cream highlights, fine grain. Photography is
  contrasty, often half-silhouetted, never beauty-lit.
- **Forbidden imagery:** ring-light beauty lighting, white
  cycloramas, glossy product gradients, stock-photo "diversity" sets.
- Repeating texture allowed: subtle film grain (2-3px noise, 4-8%
  opacity). No tile-able patterns, no mesh gradients.

### Animation & state

- **Motion is sparing.** 120-220ms. The only easing is
  `cubic-bezier(0.2, 0.8, 0.2, 1)` (ease-out). No bounces, no
  springs, no parallax.
- **Hover (Void surfaces):** lift to `--void-78` (+8% lightness).
- **Hover (Signal):** shift to `--signal-pressed` (`#D43A05`).
- **Press:** `inset 0 0 0 2px Signal` outline + 1px translateY.
- **Focus:** 2px Signal outline at 2px offset. Visible always.

### Shadows, transparency, blur

- **Depth is contrast, not blur.** Default to a 2-3px Signal rule or
  flat color block over a drop shadow.
- One sanctioned shadow: `--shadow-lift` (`0 12px 32px rgba(0,0,0,0.6)`)
  — for floating cards on Void only, used sparingly.
- Transparency / backdrop-blur: only on the Night Owl scrim
  (`rgba(10,10,10,0.72)` over photography for header bars on hero
  imagery).

### Cards

Default card: `--bg-card` fill (`#1B1B1B`), 0 radius, **no border**,
or 1px Concrete divider. Optional Signal stamp (`box-shadow: 0 0 0 3px
var(--signal-orange)`) for "active / hero" cards. No drop shadow.

---

## Content fundamentals

### Voice

**Confident. Industrial. Rooted. Mythic. Founder-direct.**

The voice writes like a duo who built something with their hands and
will tell you about it without smiling. It is not corporate. It is
not aspirational-influencer. It addresses *you* but rarely uses "we"
unless making a promise.

### Casing & punctuation

- **UPPERCASE** for display headers, eyebrows, pillar tags, and the
  occasional one-word stamp ("LIVE", "SOLD OUT", "INNER CIRCLE").
- **Sentence case** for body copy.
- **Title Case** is not used.
- Em dashes — yes. Semicolons — sparingly. Exclamation marks — no.
- Periods at end of headlines are optional but lean *no period* for
  posters/social, *period* for editorial.

### Examples (drawn from spec posture)

Good:
- "Afrohouse to the moon."
- "Night Owl Sound."
- "Inner Circle. By invitation."
- "Coordinates 001 — Nairobi."
- "Built in Kampala. Played at 2am."

Avoid:
- "Welcome to Mozaka! 🚀✨"
- "We're so excited to share..."
- "Join our community of music lovers"
- "🔥 NEW DROP 🔥"

### Pronouns

- "You" — used directly to the listener.
- "We" — reserved for promises and credits ("We make Afrohouse for
  the night.").
- "I" — only in founder voice (David or Kava speaking by name).

### Emoji

**Not part of the brand.** Do not use in product copy, posters,
social captions, decks. Exception: a single 🪐 may appear in
internal team contexts as shorthand for "to the moon" — never in
public-facing surfaces.

### Vibe checks

If a sentence could appear on a cosmetics ad, a SaaS landing page,
or a Kid's TikTok, rewrite it. If it could appear on a back-pocket
matchbook from a 2am club, you're close.

---

## Iconography

**Mozaka does not have its own icon system.** The brand leans on
*type, photography, and the helmet/wordmark marks* to do the work
icons usually do.

When functional UI icons are unavoidable (player controls, share,
close, menu, etc.), use **Lucide** via CDN at **1.5px stroke**, in
`currentColor`. Stroke icons only — never filled. Sized 16/20/24.

```html
<script src="https://unpkg.com/lucide@latest"></script>
<i data-lucide="play" style="width:20px;height:20px;color:var(--accent)"></i>
```

**Forbidden:** colored multi-tone icons, glyph-style icon fonts with
their own personality (e.g. Material's filled set), emoji as icons,
unicode symbols (★ ✓ ✕) used in place of real icons.

**The astronaut helmet is the brand's only true icon.** Use the
Helmet Glyph (`assets/logos/helmet-crest-*.png`) wherever an avatar
or app-icon-shaped mark is needed.

---

## Logo family

Three marks. All hand-cut. **Never re-vectored as a clean sans.**

1. **Helmet Crest** — astronaut helmet enclosing the wordmark.
   Primary mark. `assets/logos/helmet-crest-{signal|void|bone}.png`.
2. **Mozaka Wordmark** — hand-cut letterforms alone. Secondary.
   `assets/logos/wordmark-{signal|void|bone}.png`.
3. **Helmet Glyph** — helmet alone, wordmark removed. Mascot /
   avatar use. *(Not yet provided as a separate file — currently the
   Helmet Crest is used; flag for the team to deliver a glyph-only
   cut.)*

### Approved lockups

- **Signal-on-Void** — primary digital
- **Bone-on-Void** — quiet, editorial
- **Void-on-Signal** — high-impact poster
- **Signal-on-Bone** — print, document covers

**Never** Signal-on-Concrete (illegible at distance).

---

## Pillars (live ecosystem)

Six pillars. Tagged with the only sanctioned pill radius. **No
per-pillar color** — Signal is the accent for all of them. **No
emoji** in pillar marks anywhere public-facing.

1. **Mozaka Music** — releases, singles, Spotify
2. **Run Club** — Saturday morning, route cards, kits
3. **Orange Pill** — the rave; flyers, tickets, countdowns
4. **Camp Mozaka** — songwriting camp; passes, recap decks
5. **Coordinates** — location-reveal events; B2B sets
6. **Mozakaville** — luxury experience track; brochures, itineraries

## Catchphrases (fan language)

Set in Monument Extended. Each lives as sticker · tee · caption ·
quote card.

> Afrohouse to the Moon · Night Owl Sound · The Frequency Chose Me
> · Orange Pilled · Built on the Beat · African by Root, Global by
> Sound · We Own the Morning · Run the Rave · Mozaka Made · The
> Culture is Electronic

## Voice — tone modes & mother tongues

Four modes: **Bold** (announcements) · **Warm** (community) ·
**Poetic** (releases) · **Direct** (events).

**Luganda** and **Runyankole** appear naturally in copy — not as
aesthetic, because that's who Mozaka is. *Bwakedde* (the morning),
*Kakaaba* (the village dance) and similar are italicized in body
copy and set unquoted in display.

---

## Decisions on the Enterprise brief (merge log)

A second brief ("Mozaka — Global Afrohouse Enterprise") proposed an
expanded system. It was **merged selectively**. Adopted:
the six-pillar list, deliverables checklist, catchphrases as fan
language, four tone modes, mother-tongue policy.

**Rejected** (kept the original Night Owl discipline):
- **Six-color palette** (Neiwe Yellow, Deep Purple, Savanna Green,
  plus reframing Orange/Black/Bone). Three-color discipline stands.
  Per-pillar color is not approved.
- **Emoji in pillar names.** Not part of the brand.
- **Generic body sans (Inter / DM Sans).** SF Pro Display stands.
- **Compressed-grotesque headlines (Black Han Sans / Big Shoulders).**
  Monument Extended stands as the only display face.
- **Afro-Ndebele pattern system.** No tile-able pattern library;
  brand expresses through type, photography, helmet/wordmark, and
  Signal blocks. *Update May 2026:* four named one-off patterns
  (Helmet Tile, Spiral Chevron, Crest Halftone, Stepped Diamond)
  have been added as **commissioned graphic assets** for specific
  uses (apparel bands, packaging, cover art, linings) — not as a
  generalized fill system. The "no patterns as default decoration"
  rule still stands. New patterns are commissioned per purpose.
- **Blackletter/ornate serif accent face** for Kakaaba/Bwakedde
  releases. Mother-tongue words sit in the existing system, not in
  a separate face.
- **"Graffiti-tribal hybrid" wordmark redraw.** The hand-cut Mozaka
  wordmark already in `assets/logos/` is the wordmark. Not redrawn.

These rejections are intentional — they preserve the Night Owl
restraint that distinguishes Mozaka from generic Afrohouse visual
language. Revisit with a documented reason if needed.

## Caveats / handoff notes

- **No codebase given** — Mozaka is a music brand, not a software
  product. So this system stops at brand foundations + a
  marketing/poster UI vocabulary. There are no app or web UI kits in
  this folder. If a Mozaka.fm site or fan app is being built later,
  spin a UI kit then against the same tokens.
- **Helmet Glyph** (helmet without wordmark) was not provided as a
  standalone PNG — please supply or approve cropping the existing
  Helmet Crest.
- **Photography** — `Mozaka-Profile.png`, the Audiomack banner, and
  the duo full-body shot (`assets/photos/duo-fullbody.jpg`) are in.
  The higher-res artist pictures (`Mozaka_Artist_Picture[-2].png`,
  `Bakka_Mozaka.png`, `Kava_Mozaka.png`) failed to copy from the
  mounted folder repeatedly. Re-attach individually if needed.
- **The duo shot is on a white cyc**, which contradicts the Night
  Owl LUT. The Brand → Duo card shows three treatments: as-shot
  (flagged for internal use only), LUT-applied, and full Void
  treatment with grain. Public-facing surfaces should use the LUT
  or Void treatment — never the raw white-cyc frame.
- **PDFs not parsed** — the Roadmap, Playbook, and Coordinates PDFs
  are referenced by path but not extracted into this system. If
  specific copy or stats need to flow into mocks, point me at them.
- **Inner Circle** color reference image (`inner circle.jpg`) failed
  to copy.
