---
name: miro
description: "Create diagrams, flowcharts, and visual content on Miro boards. Use for: architecture diagrams, flowcharts, wireframes, process maps, brainstorming. Triggers: 'Miro', 'diagram', 'flowchart', 'board', 'visualize', 'create a diagram', 'architecture'."
---

# Miro - Visual Diagramming

## Overview
Miro MCP connects Claude Code to your Miro boards. Create diagrams, extract context, and manage visual content through conversation.

## Prerequisites

### Installation (Choose One)

**Option 1: Claude Code Plugin (Recommended)**
```
/plugin marketplace add miroapp/miro-ai
/plugin install miro@miro-ai
```

**Option 2: Using npx skills**
```bash
npx skills add miroapp/miro-ai
```

**Option 3: Manual MCP Config**
Add to your MCP config:
```json
{
  "mcpServers": {
    "miro": {
      "url": "https://mcp.miro.com/"
    }
  }
}
```

### Authentication
- First use prompts for OAuth login
- Grant board access in browser
- Enterprise plans need admin to enable MCP first

## Commands

| Command | What It Does |
|---------|--------------|
| `/miro:browse` | Explore board contents |
| `/miro:diagram` | Create diagrams from text |
| `/miro:doc` | Create markdown docs on boards |
| `/miro:table` | Create tables with typed columns |
| `/miro:summarize` | Extract documentation from boards |

## Use Cases for PMs

### 1. Architecture Diagrams
```
"Create a flowchart showing user authentication flow"
"Draw an ER diagram for our data model"
"Show the system architecture for the checkout process"
```

### 2. Process Maps
```
"Create a swimlane diagram for the approval workflow"
"Map out the customer support escalation process"
```

### 3. Brainstorming & Wireframes
```
"Create a wireframe for the login page"
"Set up a Kanban board structure for sprint planning"
```

### 4.提取 Board Context
```
"What's on my Miro board [URL]?"
"Summarize the architecture diagram on my board"
```

## Best Practices
- Provide clear diagram descriptions
- Specify diagram type (flowchart, ERD, sequence, etc.)
- Use proper naming for clarity
- Link boards explicitly with URLs

## Example Prompts

```markdown
"Create a flowchart on Miro showing a user login flow with:
- Login page
- Authentication check
- Success/failure paths
- Redirect to dashboard"

"Draw a sequence diagram for the checkout process:
- User adds to cart
- Payment initiation
- Payment confirmation
- Order creation"

"What's on my Miro board https://miro.com/app/board/..."
```

## Troubleshooting
- If duplicate MCP servers, remove manual config
- Enterprise: check admin enabled MCP server
- Restart Claude Code after installation
