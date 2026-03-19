---
name: shadcn-ui
description: "Use shadcn/ui component library for React. Best for: modern, accessible, customizable UI components. Triggers: 'shadcn', 'use a component', 'button', 'dialog', 'dropdown', 'form'."
---

# shadcn/ui Component Library

## Overview
shadcn/ui is a collection of re-usable components built with Radix UI and Tailwind CSS. Components are copied into your project - you own the code.

## Key Components for PMs

### Forms & Inputs
- `Input` - Text fields
- `Textarea` - Multi-line text
- `Select` - Dropdowns
- `Checkbox`, `Radio`, `Switch` - Binary inputs
- `Form` - Complex form handling with react-hook-form

### Layout
- `Card` - Content containers
- `Sheet` - Slide-out panels (like mobile menus)
- `Dialog` - Modal popups
- `Drawer` - Alternative to dialogs
- `Accordion` - Collapsible sections

### Data Display
- `Table` - Data tables
- `Badge` - Status indicators
- `Avatar` - User images
- `Calendar` - Date picker

### Feedback
- `Toast` - Temporary notifications
- `Alert` - Inline warnings/info
- `Progress` - Progress bars
- `Skeleton` - Loading states

## Installation
```bash
npx shadcn@latest add button card dialog input
```

## Usage Pattern
```jsx
import { Button } from "@/components/ui/button"
import { Card, CardHeader, CardTitle, CardContent } from "@/components/ui/card"

<Card>
  <CardHeader>
    <CardTitle>Title</CardTitle>
  </CardHeader>
  <CardContent>
    Content here
  </CardContent>
</Card>
```

## Why shadcn/ui?
- Accessible by default (WCAG)
- Customizable via Tailwind
- Lightweight (no heavy library)
- Yours to modify
