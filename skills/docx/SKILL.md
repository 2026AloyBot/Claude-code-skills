---
name: docx
description: "Create, edit, and analyze Word documents. Use for: reports, memos, letters, proposals, resumes, any .docx file. Triggers: 'Word doc', '.docx', 'create a document', 'write up', 'document with headings/tables/formatting'."
---

# DOCX - Word Document Skills

## When to Use
- Creating professional documents (reports, memos, proposals)
- Editing existing .docx files
- Adding tables, headers, footers, page numbers
- Working with tracked changes
- Converting content to polished Word docs

## Quick Commands

```bash
# Extract text from docx
pandoc document.docx -o output.md

# Validate a docx file
python scripts/office/validate.py doc.docx
```

## Best Practices
- Use `docx` npm package for creating new documents
- Always set explicit page size (default is A4, not US Letter)
- Use Arial as default font (universally supported)
- Use proper heading styles for TOC generation
- Never use unicode bullets - use proper list formatting

## Common PM Use Cases
- Product requirement documents (PRDs)
- Status reports
- Meeting notes
- Proposals
- resumes/CVs
