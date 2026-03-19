---
name: drawio
description: "Create professional diagrams in draw.io. Use for: architecture diagrams, flowcharts, network diagrams, UML. Triggers: 'draw.io', 'diagram', 'draw this', 'create diagram', 'architecture', 'flowchart'."
---

# Draw.io - Professional Diagrams

## Overview
Create editable diagrams in draw.io format. Diagrams can be embedded in Confluence, exported to PNG/SVG/PDF, or opened directly in the draw.io editor.

## Installation Options

### Option 1: MCP Server (Recommended for Claude Code)
```bash
# Install the draw.io MCP server
npx @drawio/mcp
```

### Option 2: MCP App (Inline Previews)
Add as remote MCP server:
```
https://mcp.draw.io/mcp
```

### Option 3: No Install - Just Use Skill
The skill file teaches Claude Code to generate .drawio XML directly.

## Usage

### Basic Diagram Request
```
"Create a flowchart showing user authentication flow in draw.io"
"Draw an architecture diagram for a microservices system"
"Create a network diagram with load balancer and servers"
```

### Export Formats
Request specific format:
- `/drawio` - Opens in draw.io editor
- `/drawio png` - Exports PNG (embedded, editable)
- `/drawio svg` - Exports SVG
- `/drawio pdf` - Exports PDF

## Diagram Types

### 1. Flowcharts
- Process boxes, decisions, arrows
- Swimlanes for multiple actors
- Connectors and labels

### 2. Architecture Diagrams
- AWS/Azure/GCP icons
- Servers, databases, APIs
- Data flow arrows

### 3. UML Diagrams
- Class diagrams
- Sequence diagrams
- State diagrams

### 4. Network Diagrams
- Firewalls, routers
- Cloud services
- Load balancers

### 5. Mind Maps
- Central topic
- Branching ideas
- Visual hierarchy

## Embedding in Confluence

### Method 1: PNG Export with Embed
1. Create diagram in draw.io
2. Export as PNG with "Embed Diagram" option
3. Upload to Confluence as attachment
4. Use `{drawio}` macro or insert image

### Method 2: Draw.io Macro
1. Install draw.io app in Confluence
2. Use `{drawio}` macro in page
3. Select or create diagram

### Method 3: Link to draw.io
1. Create diagram, save to cloud
2. Copy share link
3. Add link in Confluence

## Best Practices

1. **Use standard shapes** - Consistency across diagrams
2. **Add labels** - Arrow labels explain flow
3. **Group related elements** - Organize logically
4. **Use layers** - Separate different diagram types
5. **Export with embed** - Keeps diagram editable

## Example Prompts

```
"Create a draw.io flowchart for:
- User visits website
- Logs in or registers
- Views dashboard
- Can edit profile
- Logout option"

"Draw a system architecture diagram showing:
- Load balancer
- 3 web servers
- 1 database
- Redis cache
- CDN in front"

"Create a swimlane diagram for order processing:
- Customer lane
- System lane
- Warehouse lane"
```

## Tools

- [draw.io](https://draw.io) - Free online editor
- [draw.io Desktop](https://github.com/jgraph/drawio-desktop) - Desktop app
- [drawio-mcp](https://github.com/jgraph/drawio-mcp) - Official MCP server
