# Claude Code Skills for Product Managers

A curated collection of Claude Code skills to boost your productivity as a PM.

## What's Inside

| Skill | Use For |
|-------|---------|
| **docx** | Word documents - reports, PRDs, proposals |
| **pptx** | PowerPoint - presentations, decks |
| **xlsx** | Excel - trackers, dashboards, calculators |
| **frontend-design** | Avoid AI slop, create distinctive UIs |
| **shadcn-ui** | Modern React components |
| **internal-comms** | Status reports, team updates |
| **planning** | Project breakdowns, roadmaps |

## Installation

### Option 1: Clone to Your Claude Code Skills Directory

```bash
# Find your Claude Code skills directory
# Usually: ~/.claude/skills/ or ~/Library/Application Support/Claude/skills/

# Clone this repo into it
git clone https://github.com/2026AloyBot/Claude-code-skills.git ~/.claude/skills/jeff-pm-skills
```

### Option 2: Copy Individual Skills

Copy any `skills/*/SKILL.md` folder to your project's `.claude/skills/` directory.

### Option 3: Add to Existing Project

```bash
# In your project directory
mkdir -p .claude/skills
cp -r /path/to/Claude-code-skills/skills/* .claude/skills/
```

## Usage

Skills activate automatically when relevant. You can also invoke them:
- Type `/skill-name` if the skill has an argument-hint
- Or just describe what you need: "Create a status report as a Word doc"

## Requirements

- Claude Code installed
- For docx/pptx/xlsx: Node.js and relevant packages:
  ```bash
  npm install -g docx pptxgenjs xlsx
  ```

## Customize

Feel free to modify these skills for your specific needs. The SKILL.md files are yours to edit.

## Credits

Skills inspired by:
- [anthropics/skills](https://github.com/anthropics/skills)
- [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills)
