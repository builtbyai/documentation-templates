# Mermaid Diagrams Template

**Purpose**: Complete library of Mermaid diagram syntax for markdown
**Source**: Compiled from 6 Obsidian vault templates
**Usage**: Copy and customize these diagrams for your documentation

---

## Table of Contents
1. [Gantt Charts](#gantt-charts)
2. [Flowcharts (Graph TD)](#flowcharts-graph-td)
3. [Sequence Diagrams](#sequence-diagrams)
4. [Timeline Diagrams](#timeline-diagrams)
5. [Mindmaps](#mindmaps)
6. [Git Graphs](#git-graphs)
7. [Block Diagrams](#block-diagrams)

---

## Gantt Charts

### Basic Project Timeline
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Project Timeline
    section Phase 1
    Task 1           :done,    des1, 2024-01-01, 2024-01-15
    Task 2           :active,  des2, 2024-01-16, 2024-01-30
    section Phase 2
    Task 3           :         des3, 2024-02-01, 2024-02-15
    Task 4           :         des4, 2024-02-16, 2024-02-28
```

### Activity Schedule with Critical Path
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Activity Schedule
    section Upcoming
    Meeting          :done, 2024-06-12, 2024-06-12
    Task Review      :crit, active, 2024-06-12, 2024-06-12
    Code Review      :active, 2024-06-13, 2024-06-13
    section This Week
    Development      :2024-06-14, 7d
    Testing          :crit, 2024-06-21, 3d
    Deployment       :2024-06-24, 1d
```

### Multi-Section Project Plan
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Software Development Lifecycle
    section Requirements
    Gather Requirements    :done, req1, 2024-01-01, 10d
    Requirements Review    :done, req2, after req1, 5d
    section Design
    System Design          :active, des1, after req2, 15d
    Database Design        :active, des2, after req2, 10d
    section Development
    Backend Development    :dev1, after des1, 30d
    Frontend Development   :dev2, after des1, 30d
    section Testing
    Unit Testing          :test1, after dev1, 10d
    Integration Testing   :test2, after dev2, 10d
    UAT                   :crit, test3, after test2, 7d
```

**Gantt Syntax Reference**:
- `done` - Completed task (grey)
- `active` - Currently in progress (blue)
- `crit` - Critical path task (red)
- `after taskID` - Start after another task
- Dates: `YYYY-MM-DD` or `YYYY-MM-DD, Xd` (X days duration)

---

## Flowcharts (Graph TD)

### Top-Down Decision Flow
```mermaid
graph TD
    A[Start] --> B{Decision Point}
    B -->|Option 1| C[Process A]
    B -->|Option 2| D[Process B]
    C --> E[End]
    D --> E
```

### Complex System Architecture
```mermaid
graph TD
    A[User Interface] --> B[API Gateway]
    B --> C[Authentication Service]
    B --> D[Business Logic]
    D --> E[Database]
    D --> F[Cache Layer]
    C --> G[(User DB)]
    E --> H[(Main DB)]
    F --> I[(Redis)]

    style A fill:#667eea,color:#fff
    style B fill:#764ba2,color:#fff
    style C fill:#f093fb,color:#fff
    style D fill:#f5576c,color:#fff
```

### Information Architecture Flow
```mermaid
graph TD
    A[Information Architecture] --> B[Users]
    A --> C[Content]
    A --> D[Context]
    B --> E[Needs & Goals]
    B --> F[Mental Models]
    C --> G[Structure]
    C --> H[Organization]
    C --> I[Media]
    D --> J[Environment]
    D --> K[Circumstances]

    style A fill:#ff416c,color:#fff
    style B fill:#667eea,color:#fff
    style C fill:#f093fb,color:#fff
    style D fill:#43e97b,color:#fff
```

**Flowchart Syntax**:
- `graph TD` - Top to bottom
- `graph LR` - Left to right
- `[Text]` - Rectangle
- `{Text}` - Diamond (decision)
- `([Text])` - Stadium shape
- `[(Text)]` - Cylinder (database)
- `-->` - Arrow
- `-->|Label|` - Labeled arrow
- `style NodeID fill:#color,color:#textcolor` - Custom styling

---

## Sequence Diagrams

### Basic User Authentication
```mermaid
sequenceDiagram
    participant User
    participant Frontend
    participant API
    participant Database

    User->>Frontend: Enter credentials
    Frontend->>API: POST /auth/login
    API->>Database: Verify credentials
    Database-->>API: User data
    API-->>Frontend: JWT token
    Frontend-->>User: Login success
```

### Complex API Interaction
```mermaid
sequenceDiagram
    participant Client
    participant Gateway
    participant Auth
    participant Service
    participant DB

    Client->>Gateway: Request with token
    Gateway->>Auth: Validate token
    Auth-->>Gateway: Token valid
    Gateway->>Service: Forward request
    Service->>DB: Query data
    DB-->>Service: Return data
    Service-->>Gateway: Response
    Gateway-->>Client: Final response

    Note over Client,Gateway: HTTPS Connection
    Note over Gateway,Service: Internal Network
```

### Error Handling Flow
```mermaid
sequenceDiagram
    participant User
    participant App
    participant API
    participant ErrorHandler

    User->>App: Submit form
    App->>API: POST /submit
    API-->>App: 400 Bad Request
    App->>ErrorHandler: Process error
    ErrorHandler-->>App: User-friendly message
    App-->>User: Show error message
    User->>App: Correct and resubmit
    App->>API: POST /submit
    API-->>App: 200 OK
    App-->>User: Success notification
```

**Sequence Diagram Syntax**:
- `participant Name` - Define participants
- `->` - Solid line
- `-->` - Dotted line
- `->>` - Solid arrow
- `-->>` - Dotted arrow
- `Note over A,B: Text` - Add notes
- `activate/deactivate` - Show active periods

---

## Timeline Diagrams

### Project Milestones
```mermaid
timeline
    title Project Development Timeline
    section 2024 Q1
        January : Requirements Gathering
                : Stakeholder Interviews
        February : Design Phase
                 : Prototype Development
        March : Development Sprint 1
              : Development Sprint 2
    section 2024 Q2
        April : Testing Phase
              : Bug Fixes
        May : User Acceptance Testing
            : Documentation
        June : Production Deployment
             : Post-Launch Support
```

### Product Evolution
```mermaid
timeline
    title Product Evolution
    section Version 1.0
        2023-01 : Initial Release
                : Basic Features
    section Version 2.0
        2023-06 : Major Update
                : New UI
                : Performance Improvements
    section Version 3.0
        2024-01 : Enterprise Features
                : Advanced Analytics
                : API Integration
```

---

## Mindmaps

### Project Planning Mindmap
```mermaid
mindmap
  root((Project))
    Planning
      Requirements
      Timeline
      Budget
    Development
      Frontend
      Backend
      Database
    Testing
      Unit Tests
      Integration Tests
      E2E Tests
    Deployment
      Staging
      Production
      Monitoring
```

### Knowledge Organization
```mermaid
mindmap
  root((Knowledge Base))
    Documentation
      Technical Docs
      API Reference
      User Guides
    Code
      Frontend
        React
        Vue
      Backend
        Node.js
        Python
    Resources
      Tools
      Libraries
      Frameworks
```

---

## Git Graphs

### Simple Git Workflow
```mermaid
gitGraph
    commit id: "Initial commit"
    commit id: "Add features"
    branch develop
    checkout develop
    commit id: "Dev work"
    checkout main
    merge develop
    commit id: "Release v1.0"
```

### Complex Branching Strategy
```mermaid
gitGraph
    commit id: "Initial"
    commit id: "Setup"
    branch develop
    checkout develop
    commit id: "Feature scaffolding"
    branch feature-login
    checkout feature-login
    commit id: "Login UI"
    commit id: "Auth logic"
    checkout develop
    merge feature-login
    branch feature-dashboard
    checkout feature-dashboard
    commit id: "Dashboard layout"
    commit id: "Data integration"
    checkout develop
    merge feature-dashboard
    checkout main
    merge develop tag: "v1.0.0"
```

---

## Block Diagrams

### System Components (Beta Feature)
```mermaid
block-beta
    columns 3
    Frontend:3
    block:API:2
        Gateway
        Auth
    end
    Database

    Frontend --> Gateway
    Gateway --> Database
    Gateway --> Auth
```

### Data Flow Architecture
```mermaid
block-beta
    columns 4
    Input["User Input"]:1
    Process["Processing Layer"]:2
    Output["Results"]:1

    Input --> Process
    Process --> Output
```

---

## Best Practices

### General Guidelines
1. **Use Descriptive IDs**: Name nodes clearly (e.g., `userAuth` instead of `n1`)
2. **Keep It Simple**: Don't overcomplicate diagrams - break complex flows into multiple diagrams
3. **Add Context**: Use notes and labels to explain non-obvious connections
4. **Consistent Styling**: Use color schemes consistently across related diagrams
5. **Test Rendering**: Always preview diagrams in your markdown renderer

### Gantt Charts
- Use `crit` for critical path items
- Group related tasks with sections
- Keep date format consistent
- Use `after` dependencies when tasks are sequential

### Flowcharts
- Use shape meanings consistently (diamond for decisions, cylinder for databases)
- Add styling to highlight important nodes
- Keep arrows flowing in one primary direction (top-down or left-right)
- Use subgraphs for complex subsystems

### Sequence Diagrams
- Order participants logically (user → frontend → backend → database)
- Use solid lines for requests, dotted for responses
- Add notes for important context
- Show error paths explicitly

### Color Schemes
```
Professional Blues: #667eea, #764ba2
Warm Gradients: #ff416c, #ff4b2b
Success Green: #11998e, #38ef7d
Cool Blues: #4facfe, #00f2fe
Pink Purple: #f093fb, #f5576c
```

---

## Mermaid Syntax Quick Reference

### Common Shapes
```
[Rectangle]
(Rounded Rectangle)
([Stadium])
{Diamond}
{{Hexagon}}
[(Database)]
((Circle))
```

### Arrow Types
```
-->  Solid line with arrow
---  Solid line without arrow
-.-> Dotted line with arrow
-.-  Dotted line without arrow
==>  Thick line with arrow
===  Thick line without arrow
```

### Styling
```
style nodeId fill:#color,stroke:#color,color:#textcolor
classDef className fill:#color,stroke:#color
class nodeId className
```

---

**Template Version**: 1.0
**Last Updated**: 2025-12-28
**Mermaid Version**: Compatible with v10+
**Source Files**: 6 Obsidian markdown templates
