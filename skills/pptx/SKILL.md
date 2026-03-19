---
name: pptx
description: "Create, edit, and analyze PowerPoint presentations. Use for: slides, decks, presentations, pitch decks, status updates. Triggers: 'PowerPoint', 'slides', 'presentation', 'deck', '.pptx'."
---

# PPTX - PowerPoint Skills

## When to Use
- Creating presentations from scratch
- Editing existing .pptx files
- Building slide decks with charts and layouts
- Converting content to slides
- Automated slide generation

## Quick Start
Use `pptxgenjs` for programmatic creation:
```javascript
const PptxGenJS = require("pptxgenjs");
let pres = new PptxGenJS();
let slide = pres.addSlide();
slide.addText("Title", { x:1, y:1, w:8, h:1, fontSize:24, bold:true });
pres.writeFile({ fileName: "presentation.pptx" });
```

## Best Practices
- Keep slides simple - one main idea per slide
- Use consistent color scheme
- Include visual hierarchy
- Add speaker notes for presentation context

## Common PM Use Cases
- Quarterly business reviews
- Product demos
- Stakeholder updates
- Board presentations
- Project kickoffs
