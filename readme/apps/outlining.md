# Creating Outlines in Joplin

Joplin supports creating structured outlines within notes using Markdown's hierarchical list syntax. While Joplin is not a dedicated outliner like Workflowy or Dynalist, it provides powerful outlining capabilities through nested lists that can help you organize thoughts, projects, and hierarchical information.

## Basic Outlining with Markdown

Joplin uses standard Markdown for creating outlines. You can create nested bullet lists and numbered lists by indenting with spaces or tabs.

### Unordered (Bullet) Lists

Create bullet list outlines by using `-`, `*`, or `+` followed by a space. Indent sub-items with 4 spaces or a tab:

```markdown
- Top level item
    - Second level item
    - Another second level item
        - Third level item
        - Another third level item
    - Back to second level
- Another top level item
```

**Renders as:**

- Top level item
    - Second level item
    - Another second level item
        - Third level item
        - Another third level item
    - Back to second level
- Another top level item

### Ordered (Numbered) Lists

Create numbered outlines using `1.`, `2.`, etc. followed by a space. Indent sub-items similarly:

```markdown
1. Introduction
2. Main topic
    1. First sub-topic
    2. Second sub-topic
        1. Detailed point
        2. Another detailed point
    3. Third sub-topic
3. Conclusion
```

**Renders as:**

1. Introduction
2. Main topic
    1. First sub-topic
    2. Second sub-topic
        1. Detailed point
        2. Another detailed point
    3. Third sub-topic
3. Conclusion

### Task Lists with Checkboxes

For project management and to-do list outlines, use checkbox syntax:

```markdown
- [ ] Project planning
    - [x] Define requirements
    - [x] Create timeline
    - [ ] Budget approval
        - [x] Submit proposal
        - [ ] Wait for response
- [ ] Implementation phase
    - [ ] Development
    - [ ] Testing
```

**Renders as:**

- [ ] Project planning
    - [x] Define requirements
    - [x] Create timeline
    - [ ] Budget approval
        - [x] Submit proposal
        - [ ] Wait for response
- [ ] Implementation phase
    - [ ] Development
    - [ ] Testing

**Note:** Checkboxes can be ticked directly in both the desktop and mobile applications, making them perfect for interactive task management.

## Tips for Effective Outlining

### 1. Consistent Indentation

Use consistent indentation (4 spaces or 1 tab per level) for clean, readable outlines:

```markdown
- Level 1
    - Level 2 (4 spaces)
        - Level 3 (8 spaces)
            - Level 4 (12 spaces)
```

### 2. Mix List Types with Separation

While you cannot mix bullet types within a single continuous list (a Markdown limitation), you can separate different list types with horizontal rules or blank lines:

```markdown
## Project Tasks

- [ ] Design phase
    - [ ] Create mockups
    - [ ] Get approval

---

### Requirements

1. User requirements
    - Authentication system
    - Dashboard interface
2. Technical requirements
    - Database setup
    - API endpoints
```

### 3. Use Headings to Organize Sections

Combine headings with outlines to create well-structured documents:

```markdown
# Project Plan

## Phase 1: Research
- Market analysis
    - Competitor research
    - User surveys
- Technology review
    - Frontend options
    - Backend options

## Phase 2: Development
- Sprint 1
    - User authentication
    - Basic UI
- Sprint 2
    - Core features
    - Testing
```

### 4. Add Context with Regular Text

Enhance your outlines with explanatory paragraphs:

```markdown
## Meeting Notes - January 15, 2024

The team discussed the following action items:

- [ ] Marketing campaign
    - [ ] Design assets
    - [ ] Copy writing
    - [ ] Schedule posts

Next steps: Review progress in next week's meeting.
```

## Rich Text Editor Considerations

If you use the Rich Text editor, outlining works similarly:

- Create lists using the toolbar buttons or keyboard shortcuts
- Press <kbd>Tab</kbd> to indent (create sub-items)
- Press <kbd>Shift+Tab</kbd> to outdent (move back to parent level)
- Type `- ` at the start of a line to begin a bullet list
- Type `1. ` at the start of a line to begin a numbered list

**Important:** All list items in a continuous list must be of the same type (all bullets, all numbers, or all checkboxes) when using the Rich Text editor. To use different types, separate them with horizontal rules or blank lines.

## Advanced Outlining Techniques

### Collapsible Sections with HTML

For very large outlines, you can use HTML `<details>` tags to create collapsible sections:

```html
<details>
<summary>Click to expand: Project Details</summary>

- Budget: $10,000
- Timeline: 6 months
- Team size: 5 people
    - 2 developers
    - 1 designer
    - 1 project manager
    - 1 QA tester

</details>
```

### Linking Between Notes

Create a hierarchical knowledge base by linking related outline notes:

```markdown
# Main Project Overview

- Planning phase - [See detailed plan](:/abc123...)
- Execution phase - [See execution notes](:/def456...)
- Review phase - [See review criteria](:/ghi789...)
```

To get the link to a note:
- **Desktop**: Right-click on a note and select "Copy Markdown link"
- **Mobile**: Open the note, tap the ⋮ menu, and select "Copy Markdown link"

## Common Use Cases

### 1. Project Planning

```markdown
# Website Redesign Project

- [ ] Discovery
    - [x] Stakeholder interviews
    - [x] Analytics review
    - [ ] User testing
- [ ] Design
    - [ ] Wireframes
    - [ ] Visual design
    - [ ] Prototype
- [ ] Development
    - [ ] Frontend
    - [ ] Backend
    - [ ] Integration
- [ ] Launch
    - [ ] Testing
    - [ ] Deployment
    - [ ] Monitoring
```

### 2. Note-Taking and Learning

```markdown
# Biology - Cell Structure

1. Prokaryotic Cells
    - Characteristics
        - No nucleus
        - Simple structure
    - Examples
        - Bacteria
        - Archaea
2. Eukaryotic Cells
    - Characteristics
        - Has nucleus
        - Complex organelles
    - Examples
        - Animal cells
        - Plant cells
            - Has cell wall
            - Contains chloroplasts
```

### 3. Meeting Minutes

```markdown
# Weekly Team Meeting - Feb 1, 2024

## Attendees
- John (PM)
- Sarah (Dev)
- Mike (Design)

## Discussion Points
1. Project status
    - Development: 80% complete
    - Design: Finalizing assets
2. Blockers
    - API integration delayed
        - Waiting on vendor
        - Target: Next week
3. Action items
    - [ ] John: Follow up with vendor
    - [ ] Sarah: Document API requirements
    - [ ] Mike: Prepare presentation
```

### 4. Content Planning

```markdown
# Blog Post Ideas

- Technical tutorials
    - Getting started with Docker
        - Installation
        - Basic commands
        - Example project
    - Understanding REST APIs
        - HTTP methods
        - Status codes
        - Best practices
- Product updates
    - New feature announcements
    - Behind the scenes
    - User success stories
```

## Differences from Dedicated Outliners

While Joplin's outlining is powerful, it's important to understand how it differs from dedicated outlining tools like Workflowy:

| Feature | Joplin | Dedicated Outliners (e.g., Workflowy) |
|---------|--------|--------------------------------------|
| Nested lists | ✅ Supported | ✅ Supported |
| Keyboard navigation | ⚠️ Basic (Tab/Shift+Tab) | ✅ Advanced (Alt+Arrow, etc.) |
| Collapsible items | ⚠️ Via HTML `<details>` | ✅ Built-in |
| Hoisting/Focus | ❌ Not available | ✅ Available |
| Zoom into items | ❌ Not available | ✅ Available |
| Tags on items | ❌ Note-level only | ✅ Item-level |
| Multiple panes | ❌ Single note view | ⚠️ Varies |

**Strengths of Joplin for outlining:**
- Standard Markdown format (portable and future-proof)
- Rich text editing option
- Integrated with full note-taking features
- Attachment support
- Powerful search
- End-to-end encryption
- Free and open source

## Plugins for Enhanced Outlining

You can extend Joplin's outlining capabilities with community plugins. Visit the plugin repository or check the [Joplin Forum](https://discourse.joplinapp.org/) for:

- Outline navigation plugins
- Table of contents generators
- Folding/collapsing plugins
- Outliner-specific themes

To install plugins:
1. Go to **Tools > Options > Plugins** (Desktop)
2. Search for outlining-related plugins
3. Install and configure as needed

## Keyboard Shortcuts

Useful shortcuts for working with outlines:

**Desktop:**
- <kbd>Ctrl/Cmd + ]</kbd>: Indent list item (in Markdown editor)
- <kbd>Ctrl/Cmd + [</kbd>: Outdent list item (in Markdown editor)
- <kbd>Tab</kbd>: Indent (in Rich Text editor)
- <kbd>Shift + Tab</kbd>: Outdent (in Rich Text editor)
- <kbd>Ctrl/Cmd + L</kbd>: Toggle checkboxes

**Mobile:**
- Use the toolbar buttons for list formatting
- Long-press for additional options

## Summary

Joplin provides robust outlining capabilities through Markdown's hierarchical list syntax. While it may not have all the specialized features of dedicated outlining tools, it excels at combining outlining with full note-taking features, making it perfect for:

- Project management and planning
- Hierarchical note-taking
- Task management with checkboxes
- Structured documentation
- Knowledge organization

The standard Markdown format ensures your outlines remain portable and readable in any Markdown editor, while Joplin's sync and search capabilities make your outlined information accessible across all your devices.

For users coming from Workflowy or similar tools, the key difference is that Joplin treats outlines as content within notes rather than as the primary organizational structure. This makes it ideal for combining prose, images, code blocks, and structured outlines in a single, cohesive note.
