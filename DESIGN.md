# MRCEM Exam Prep — Design System

## Philosophy

This course is a reading-to-learn experience. The design must feel like a premium publication — every.to's literary elegance, Notion's calm spaciousness, Linear's precision. Content density without visual noise. Beauty that recedes into the background so the material commands attention.

## Principles

### 1. Typography is the architecture
- **Body:** Charter / Georgia serif at 17–18px — warm, readable, authoritative. Every.to uses serif body for its magazine feel; we do the same for sustained reading.
- **UI:** System font stack (Inter / SF Pro / Segoe UI) for navigation, badges, metadata — the crisp precision of Linear.
- **Scale:** A restrained scale — h1 at 2.2rem, h2 at 1.4rem, h3 at 1.15rem. No typographic shouting.
- **Measure:** 760px max-width, 1.65 line-height. Comfortable for long-form medical reading.

### 2. Space is the luxury material
- Generous padding. Cards breathe. Sections have room.
- Notion's genius is what it *doesn't* show. Remove chrome. Thin dividers, not heavy borders.
- Whitespace is the primary layout tool — not boxes.

### 3. One accent color. Everything else is neutral.
- Linear uses a single blue accent against cool grays. We adopt the same discipline.
- **Accent:** #4f46e5 (indigo) for links, active states, highlights
- **Success:** #059669 for correct answers
- **Danger:** #dc2626 for incorrect
- **Warning:** #d97706 for alerts
- Everything else: neutral-50 through neutral-900

### 4. Micro-interactions signal quality
- Every interactive element has a smooth CSS transition (150–250ms)
- Hover states are subtle lifts (translateY(-1px) + shadow increase)
- Links underline on hover with a slide-in effect
- Quiz options smoothly transition border/background
- Flashcards have a gentle flip
- Status badges scale subtly on hover
- Page sections fade in on load

### 5. Content-first, chrome-last
- Remove everything that's not content or essential navigation
- The quick-launch nav buttons are gone — the lesson list IS the navigation
- Status badges tell you what's ready vs upcoming at a glance
- The countdown is minimal — a single number, not a banner

### 6. Print is a first-class medium
- Print styles strip color, remove interactive elements, maximize readability
- These are study materials — many users will print them

## Color Palette

```
Base:
  --bg:           #fafbfc    page background
  --surface:      #ffffff    card backgrounds
  --border:       #e5e7eb    subtle borders
  --border-light: #f3f4f6    very subtle dividers

Text:
  --text:         #111827    primary text
  --text-muted:   #6b7280    secondary text
  --text-subtle:  #9ca3af    tertiary / placeholder

Accent:
  --accent:       #4f46e5    links, active, brand
  --accent-hover: #4338ca    hover state
  --accent-light: #eef2ff    accent backgrounds

Semantic:
  --success:      #059669    correct answers
  --success-bg:   #d1fae5
  --danger:       #dc2626    incorrect answers
  --danger-bg:    #fee2e2
  --warning:      #d97706    alerts / deadlines
  --warning-bg:   #fef3c7
  --info:         #2563eb    blueprint context
  --info-bg:      #dbeafe

Shadows:
  --shadow-sm:    0 1px 2px rgba(0,0,0,0.05)
  --shadow-md:    0 4px 6px -1px rgba(0,0,0,0.07)
  --shadow-lg:    0 10px 25px -5px rgba(0,0,0,0.08)
```

## Typography Scale

| Element | Font | Size | Weight | Notes |
|---------|------|------|--------|-------|
| h1 | Charter | 2.2rem | 700 | Page titles |
| h2 | Charter | 1.4rem | 600 | Section headers with thin bottom border |
| h3 | Charter | 1.15rem | 600 | Sub-sections |
| body | Charter | 17px | 400 | Main reading text, 1.65 line-height |
| .lesson-number | system-ui | 0.8rem | 600 | Uppercase, tracked-out, accent color |
| .lesson-meta | system-ui | 0.85rem | 400 | Muted secondary info |
| table | Charter | 0.9rem | 400 | Compact but readable |
| .status badge | system-ui | 0.72rem | 500 | Tiny, rounded-pill |
| footer | Charter | 0.9rem | 400 | Muted, separated by top border |

## Spacing Scale

- **xs:** 0.25rem
- **sm:** 0.5rem
- **md:** 1rem
- **lg:** 1.5rem
- **xl:** 2rem
- **2xl:** 3rem

Page container: `max-width: 760px` with `padding: 2rem 1.5rem 4rem`

## Component Patterns

### Callout Boxes (blueprint-context, exam-pattern, mnemonic, key-point, exam-tip)
- Left border accent (4px)
- Subtle background tint
- Rounded right corners (8px)
- System-ui font at 0.92rem
- Padding: 1rem 1.25rem

### Quiz Options
- 2px border, rounded 8px
- Hover: border-color transition to accent, background tint
- Correct: green border + green bg
- Incorrect: red border + red bg
- Feedback: slides in below, color-coded
- All transitions 150ms ease

### Flashcards
- Subtle gradient background
- Click to flip (instant toggle)
- Centered text
- Border 2px neutral
- Rounded 12px

### Tables
- Clean, minimal
- Header row with subtle background
- Thin borders
- Full-width

### Phase Cards (index page)
- White card, subtle border
- Rounded 12px
- Hover: translateY(-1px), shadow increase
- Transition: 200ms ease
