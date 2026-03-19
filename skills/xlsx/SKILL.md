---
name: xlsx
description: "Create, edit, and analyze Excel spreadsheets. Use for: data analysis, budgets, trackers, dashboards, tables with formulas. Triggers: 'Excel', 'spreadsheet', '.xlsx', 'sheet', 'workbook', 'formula', 'chart'."
---

# XLSX - Excel Spreadsheet Skills

## When to Use
- Creating spreadsheets with data
- Building calculators and trackers
- Adding formulas and charts
- Editing existing .xlsx files
- Data analysis and visualization

## Quick Start
Use `xlsx` (SheetJS) for programmatic creation:
```javascript
const XLSX = require("xlsx");
const ws = XLSX.utils.aoa_to_sheet([["Name", "Value"], ["Item", 100]]);
const wb = XLSX.utils.book_new();
XLSX.utils.book_append_sheet(wb, ws, "Sheet1");
XLSX.writeFile(wb, "data.xlsx");
```

## Best Practices
- Use clear headers in first row
- Keep data in tabular format (no merged cells for data)
- Use named ranges for formulas
- Format numbers appropriately

## Common PM Use Cases
- Budget tracking
- OKR dashboards
- Sprint burndown charts
- Resource allocation
- ROI calculators
