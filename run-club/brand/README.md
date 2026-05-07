# Mozaka Run Club — Brand Assets

Design system for the Saturday morning run club.
Part of the Mozaka universe — the dawn counterpart to the Night Owl Sound.

```
mozaka-run-club/brand/
├── colors.json          → machine-readable palette (pipe into any CLI tool)
├── typography.json      → font system, scale, and usage rules
├── css-variables.css    → drop into any web project
├── brand-voice.md       → copy team reference: personality, tone, sample content
├── logo-concept.md      → design brief for the Striding Sun mark
├── brand-guide.md       → master reference: color, type, photography, social, merch
└── README.md            → this file
```

---

## CLI usage

```sh
# Read the full color palette
cat colors.json | jq '.palette'

# Get just the color roles (primary, secondary, accent, etc.)
cat colors.json | jq '.roles'

# Get a specific hex value
cat colors.json | jq '.palette.volt.hex'

# Get the display font's Google Fonts URL
cat typography.json | jq '.fonts.display.url'

# Get the full type scale
cat typography.json | jq '.scale'

# Get all typography rules
cat typography.json | jq '.rules[]'

# Get all approved color pairings
cat colors.json | jq '.pairings'
```

---

## How this relates to the main Mozaka brand

The main Mozaka brand (in `2026 Roadmap/Brand/Mozaka Design System/`) runs on:
- **Void Black / Signal Orange / Concrete Grey** — three-color discipline
- **Monument Extended** — industrial, heavy, hand-cut worldmark energy
- **Night Owl Sound** — dark, Afrofuturist, late-night aesthetic

The Run Club is the dawn counterpart:
- **Dawu / Usiku / Volt** lead the palette — same restraint, warmer range
- **Big Shoulders Display** — same ultra-condensed authority as Monument, more kinetic
- **7am aesthetic** — bright, sweaty, community-facing, Nairobi-native

Same universe. Different hour.

---

## Fonts (Google Fonts)

All three fonts load from a single `@import` in `css-variables.css`:

```css
@import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@400;600;700;800;900&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,700;1,9..40,400&family=Space+Mono:ital,wght@0,400;0,700;1,400&display=swap');
```

| Role | Family | Use |
|---|---|---|
| Display | Big Shoulders Display | Headlines, event names, hero text |
| Body | DM Sans | Captions, copy, UI, WhatsApp |
| Mono | Space Mono | Times, paces, distances, stats |

---

## Quick color reference

| Name | HEX | Role |
|---|---|---|
| Dawu | `#E8632A` | Primary — dawn ember orange |
| Usiku | `#0E0B1F` | Background — deep indigo-black |
| Haraka | `#FF3B5C` | Secondary — finish line energy |
| Jua | `#FFB800` | Accent warm — solar gold |
| Pumzi | `#F5ECD7` | Light background / text-on-dark |
| Ngozi | `#C8A882` | Muted text / dividers |
| Baridi | `#1E2D3E` | Secondary surface — cool morning air |
| Volt | `#D4F000` | Cut-through accent — use sparingly |
