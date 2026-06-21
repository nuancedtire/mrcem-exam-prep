# MRCEM Exam Prep — Design System

## Philosophy

This is a reading-to-learn experience for clinicians. The design draws from three sources:

- **every.to** — bold dark/light contrast, magazine typography, editorial confidence. The hero makes a statement. The reading experience feels premium.
- **Notion** — warm whites, soft rounded cards, emoji anchors, generous spacing. Content floats on a calm surface.
- **Linear** — precision status indicators, crisp data tables, monospaced numbers. Information is scannable at a glance.

The result: a course that feels like a premium publication, not a textbook.

## Principles

### 1. Bold entry, calm reading
The hero is dark and confident — it says "this matters." The reading surface is warm and quiet — it says "stay here, focus."

### 2. Typography carries the weight
- **Headings:** Charter/Georgia serif — authoritative, warm
- **Body:** Charter/Georgia at 17px with 1.7 line-height — comfortable for sustained study
- **UI elements:** Inter/system-ui — crisp, modern, scannable
- **Numbers:** Tabular figures (`font-feature-settings: "tnum"`) for countdowns and lesson numbers

### 3. One accent. Everything else is neutral.
- Accent: warm indigo (#4f46e5) — links, hover states, active elements
- Everything else: warm grays and off-whites. No purple gradients, no rainbow semantics.
- The dark hero uses only white and transparent white — no colored text.

### 4. Warm surfaces
- Background: #faf8f5 (warm off-white — paper, not screen)
- Cards: #ffffff with subtle warm borders (#e8e5e0)
- Dark surfaces: #111827 with radial indigo glow

### 5. Micro-interactions signal care
- Cards lift 2px on hover with shadow expansion (300ms ease)
- Quiz options lift 1px + glow ring on hover (200ms)
- Answer feedback slides up (250ms)
- Flashcard flips with fade (300ms)
- Links transition color (200ms)

### 6. Print is respected
- Print strips backgrounds, borders, animations
- Body becomes 12pt black on white
- Interactive elements hidden
- Ornaments disabled

## Color Palette

```
Warm surface:   #faf8f5  (page background — warm paper)
White:          #ffffff  (cards)
Dark:           #111827  (hero, footer)
Dark glow:      radial-gradient(ellipse, rgba(79,70,229,0.12), transparent)

Text:
  heading:      #1a1a2e  (near-black with blue undertone)
  body:         #3e3e3e  (softened dark — never pure black)
  muted:        #787878  (secondary text)
  subtle:       #a3a3a3  (tertiary)

Accent:
  base:         #4f46e5  (indigo-600)
  hover:        #4338ca  (indigo-700)
  light bg:     #eef2ff  (indigo-50)
  glow ring:    rgba(79,70,229,0.08)

Borders:
  base:         #e8e5e0  (warm gray)
  light:        #f0ede8  (very subtle)

Semantic:
  success:      #059669 / bg #ecfdf5
  danger:       #dc2626 / bg #fef2f2
  warning:      #d97706 / bg #fffbeb
  info:         #2563eb / bg #eff6ff
```

## Typography Scale

| Element | Font | Size | Weight | Notes |
|---------|------|------|--------|-------|
| Hero h1 | Charter | 3rem | 700 | -0.03em letter-spacing |
| Page h1 | Charter | 2.4rem | 700 | -0.02em letter-spacing |
| h2 | Charter | 1.45rem | 600 | Preceded by "···" ornament |
| h3 | Charter | 1.15rem | 600 | |
| Body | Charter | 17px | 400 | 1.7 line-height |
| UI text | Inter | 0.75–0.9rem | 400–600 | Labels, badges, metadata |
| Kicker | Inter | 0.72rem | 600 | Uppercase, 0.15em tracking |
| Table headers | Inter | 0.72rem | 600 | Uppercase, 0.06em tracking |

## Spacing

- Page container: 720px max-width
- Hero: full-bleed dark background
- Section margin: 2.5–3rem between major sections
- Card padding: 1.5–1.75rem
- Content padding: 1.5rem horizontal

## Component Patterns

### Hero (index page only)
- Full-bleed dark (#111827) background
- Subtle radial indigo glow (CSS radial-gradient)
- White serif heading at 3rem
- Inter subtitle in 60% white
- Countdown number at 4.5rem Inter
- Application date in 55% white

### Phase Cards
- White card, 1px warm border, 16px radius
- Hover: lift 2px, shadow expands
- Inter for all card text
- Lesson list with tabular numbers, hover highlights
- Linear-style status badges (Ready / Next / Upcoming)

### Blueprint Card
- White card, centered text
- Clean table with horizontal rules only
- Progress bars: 5px tall, indigo fill at 60% opacity

### Section Headings (h2)
- Centered
- 32px indigo underline ornament
- "···" ornament above (in lesson pages)

### Callout Boxes
- Full border (not just left border), rounded
- Light tinted backgrounds
- Inter font at 0.88rem

### Quiz Options & Flashcards
- See shared CSS — consistent interactions everywhere
