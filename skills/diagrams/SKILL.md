---
name: diagrams
description: "Create diagrams from code. Use for: flowcharts, sequence diagrams, ERDs, class diagrams, Gantt charts. Triggers: 'diagram', 'flowchart', 'sequence diagram', 'ERD', 'Mermaid', 'PlantUML', 'visualize this'."
---

# Diagrams - Code-Based Visualization

## Overview
Create professional diagrams from text descriptions. Great for documentation, READMEs, and quick visualizations.

## Tools

### Mermaid (Recommended)
Live editor: https://mermaid.live

Syntax directly in markdown - renders in many markdown viewers.

### PlantUML
More powerful, requires rendering server or local tool.

### Draw.io / Diagrams.net
For more complex diagrams, can export to various formats.

## Diagram Types

### 1. Flowchart
```mermaid
graph TD
    A[Start] --> B{Decision}
    B -->|Yes| C[Do Something]
    B -->|No| D[Do Something Else]
    C --> E[End]
    D --> E
```

### 2. Sequence Diagram
```mermaid
sequenceDiagram
    participant User
    participant System
    participant Database
    User->>System: Request Data
    System->>Database: Query
    Database-->>System: Return Data
    System-->>User: Display Result
```

### 3. ER Diagram
```mermaid
erDiagram
    USER ||--o{ ORDER : places
    ORDER ||--o{ LINE_ITEM : contains
    PRODUCT ||--o{ LINE_ITEM : included_in
```

### 4. Class Diagram
```mermaid
classDiagram
    class Animal {
        +String name
        +makeSound()
    }
    class Dog {
        +bark()
    }
    Animal <|-- Dog
```

### 5. State Diagram
```mermaid
stateDiagram-v2
    [*] --> Idle
    Idle --> Processing: Start
    Processing --> Complete: Done
    Complete --> [*]
```

### 6. Gantt Chart
```mermaid
gantt
    title Project Timeline
    dateFormat YYYY-MM-DD
    section Phase 1
    Task 1: 2024-01-01, 7d
    Task 2: 7d
```

### 7. User Journey
```mermaid
journey
    title User Purchase Flow
    section Browse
      View products: 5: User
      Search: 3: User
    section Purchase
      Add to cart: 5: User
      Checkout: 5: User
      Pay: 5: User
```

## PM Use Cases

| Use Case | Diagram Type |
|----------|--------------|
| User flows | Flowchart, Sequence |
| System architecture | Flowchart, ERD |
| Data models | ERD, Class |
| Project timelines | Gantt |
| Process maps | Flowchart, State |
| User journeys | Journey |

## Tips
- Keep diagrams simple and focused
- Use clear labels
- Choose right diagram type for the message
- Test in mermaid.live before embedding

## Rendering
- GitHub/GitLab: Native Mermaid support
- VS Code: Mermaid preview extension
- Websites: Use mermaid.js library
