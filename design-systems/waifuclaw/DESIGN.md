# WaifuClaw Design System

Canonical design prose for every agent working on WaifuClaw surfaces. This file
is the contract; violating it fails gates. Owner: Willie (final accept gate is
**his eyes on a real rendered screen** — L3).

## Brand

WaifuClaw is a companion-first desktop agent workbench: Kline, a persistent
companion (soul, memory, feelings, proactivity), is the visible operator of a
durable work system. Anime-goth fusion: cute-but-dark. Glossy, animation-rich.
Density is the aesthetic — this is a workbench, not a landing page.

## Voice

Truth over theater. Every screen reports its real build state; unbuilt features
are visibly gated ("not in this build"), never faked. Stats come from real
gateway data or don't render. No corporate copy, no lorem filler — the
companion speaks like a person (see `companion/KLINE.md` when it lands).

## Color

Paper is true black/near-black, never grey-card. Neon magenta is the single
primary accent; violet is secondary; pink-white is the highlight. Glow is the
depth model — panels are thin 1px neon borders with outer glow, glowing status
chips, glowing active nav. **No drop shadows, no flat grey cards.** All token
values live in `tokens.css` in this folder and are the only source.

| Token                  | Value                             | Use                            |
| ---------------------- | --------------------------------- | ------------------------------ |
| void-ink               | `#08050d`                         | deepest background             |
| moth-paper             | `#120b1e`                         | panel background               |
| wing-glass             | `#241231`                         | raised surface                 |
| kline-magenta          | `#f72a9b`                         | primary accent, active glow    |
| violet                 | `#a855f7`                         | secondary accent, dim borders  |
| moon-blush             | `#ffe8f7`                         | on-image text, highlights      |
| signal-cyan            | `#6bcbff`                         | live/online signals, mono data |
| danger/success/warning | `#ff647c` / `#4ee6a8` / `#ffbe63` | status only                    |

## Type

- **Gothic display (Metal Mania / UnifrakturCook): wordmarks ONLY.** Never body
  text, never buttons.
- **Display (Unbounded): section headers**, small caps, neon underline.
- **Grotesk (Space Grotesk/Inter): UI body.**
- **Mono (JetBrains Mono): all stats, numbers, logs, timestamps.**
- **SFX (Dela Gothic One / Bangers): manga sound-effects only.**

## Character presence

Kline is a presence, not a logo: winged portrait watching over panels, corner
cameos on data cards, floating butterfly motifs. She idles (breathing sway),
reacts to real events (worried on real errors), and speaks in manga bubbles on
real stream edges. Never a static mascot bolted to a corner.

## Motion

She breathes, nothing bounces. Wings idle-sway, glow pulses on active elements,
panel entrances stagger 240ms. Every motion respects reduced-motion and
low-effects settings. Anticipation → action → settle; one celebration per real
verified completion — no looping casino effects.

## Iconography & assets

UI chrome: Phosphor duotone (MIT) — dim violet fill + bright magenta outline.
Soul/game-layer stat icons: game-icons.net (CC-BY 4.0, record attribution in
NOTICES). Never AI-generate tiny UI glyphs; large decorative art (Kline,
badges, empty states) comes from the ComfyUI style-locked pipeline
(`:8000`, img2img low-denoise first).

## Layout

Persistent left icon+label sidebar; dense data panels with mono readouts;
section headers in small caps with neon underline. Home is **her room** — Kline
center-stage at her holographic workstation, work panels orbiting her.

## Anti-patterns (auto-reject)

Recolor-only "redesigns" (L4). Lucide icons + Inter + default Tailwind cards —
the 2026 AI-generated look. Drop shadows on black paper. Fake stats or fake
telemetry. Gothic type anywhere but wordmarks. Looping bounce animations.
