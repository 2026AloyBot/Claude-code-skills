---
name: frontend-design
description: "Create bold, distinctive frontend designs. Avoid 'AI slop' - generic, cookie-cutter aesthetics. Use for: React, Tailwind, any web UI. Triggers: 'make it look good', 'design', 'frontend', 'UI', 'style'."
---

# Frontend Design - Avoid AI Slop

## Core Principle
Generic AI-generated UI looks the same everywhere. Your designs should feel intentional, distinctive, and premium.

## Design Rules

### 1. Choose a Bold Direction
Pick ONE strong aesthetic:
- **Brutalist**: Raw, bold typography, high contrast, sharp edges
- **Maximalist**: Rich colors, layered textures, elaborate details
- **Glassmorphism**: Frosted glass, subtle blurs, depth
- **Retro-futuristic**: Neon, grids, 80s/90s vibes
- **Minimalist Japanese**: Lots of whitespace, refined typography

### 2. Typography Matters
- Use 1-2 distinctive fonts max
- Don't just use Inter/Roboto - try something interesting
- Play with font sizes dramatically - big headlines, small labels

### 3. Color Strategy
- Pick a cohesive palette (2-3 colors max)
- Use color meaningfully, not everywhere
- Dark mode should be intentional, not just inverted

### 4. Avoid Generic Patterns
- ❌ "Modern gradient" backgrounds
- ❌ Generic "blue button with white text"
- ❌ Cookie-cutter card layouts
- ❌ Boring 16px Inter everywhere

### 5. Add Delight
- Subtle animations
- Interesting hover states
- Unique visual elements

## Implementation Tips (React + Tailwind)
```jsx
// ❌ Generic AI slop
<div className="bg-white rounded-lg shadow-md p-4">

// ✅ Intentional design
<div className="bg-slate-900/50 backdrop-blur-xl border border-white/10 rounded-2xl p-6 shadow-2xl">
```

## Reference
Inspired by the official Claude frontend-design skill - always commit to a distinctive aesthetic.
