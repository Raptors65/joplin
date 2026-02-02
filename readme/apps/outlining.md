# Outlining and Nested Lists

Joplin supports creating hierarchical outlines similar to Workflowy, using standard Markdown nested lists combined with keyboard shortcuts for quick manipulation.

## Creating Nested Lists

You can create nested lists in Joplin by indenting list items. Here's how:

### Basic Nested List Example

```markdown
- Main topic
    - Subtopic 1
    - Subtopic 2
        - Detail A
        - Detail B
    - Subtopic 3
- Another main topic
    - Another subtopic
```

This will render as:

- Main topic
    - Subtopic 1
    - Subtopic 2
        - Detail A
        - Detail B
    - Subtopic 3
- Another main topic
    - Another subtopic

### Numbered Nested Lists

```markdown
1. Introduction
2. Main topic
    1. First sub-topic
    2. Second sub-topic
        1. Detailed point
        2. Another detailed point
3. Conclusion
```

This will render as:

1. Introduction
2. Main topic
    1. First sub-topic
    2. Second sub-topic
        1. Detailed point
        2. Another detailed point
3. Conclusion

## Keyboard Shortcuts for Outlining

Joplin provides keyboard shortcuts to quickly manipulate list items, making it easy to reorganize your outlines:

### Desktop Application

| Action | Windows/Linux | macOS |
|--------|--------------|-------|
| Increase indent (move item right) | `Tab` or `Ctrl+]` | `Tab` or `Cmd+]` |
| Decrease indent (move item left) | `Shift+Tab` or `Ctrl+[` | `Shift+Tab` or `Cmd+[` |
| Toggle bullet list | `Ctrl+Alt+-` | `Option+Cmd+-` |

**Note:** To toggle numbered lists or checklists, use the toolbar buttons or command palette (press `Ctrl+Shift+P` on Windows/Linux or `Cmd+Shift+P` on macOS and search for "numbered list" or "checklist").

### Mobile Application

On mobile devices:
- Use the toolbar buttons at the top of the editor to toggle list types
- Tap at the beginning of a line and press the indent/outdent buttons in the toolbar
- Alternatively, you can manually type list markers (`-`, `1.`, `- [ ]`) and use spaces for indentation

### Tips for Effective Outlining

1. **Start with bullets**: Begin typing your outline with `-` or `*` followed by a space
2. **Use Tab to indent**: When you want to create a sub-item, press Tab at the beginning of the line
3. **Use Shift+Tab to outdent**: To move an item back to a higher level, press Shift+Tab
4. **Mix list types**: You can combine bulleted lists, numbered lists, and checklists within the same outline
5. **Use Enter to continue**: Pressing Enter automatically continues the current list format

## Using Checklists for Task Outlines

Joplin's checklist feature is particularly useful for task-oriented outlines:

```markdown
- [ ] Project planning
    - [x] Define requirements
    - [x] Create timeline
    - [ ] Assign resources
        - [ ] Developer team
        - [ ] Design team
    - [ ] Set milestones
- [ ] Implementation
    - [ ] Phase 1
    - [ ] Phase 2
```

You can check items off directly in the rendered view by clicking on the checkboxes.

## Collapsing and Expanding Sections

While Joplin doesn't have built-in list collapsing in the markdown editor, you can use:

1. **Headings with fold**: Use headings (`#`, `##`, `###`) for major sections, which can be folded in the editor
2. **Multiple notes**: Break large outlines into separate notes and link them together using [note links](https://github.com/laurent22/joplin/blob/dev/readme/apps/link_to_note.md)
3. **Subnotebooks**: Organize related outlines into [subnotebooks](https://github.com/laurent22/joplin/blob/dev/readme/apps/subnotebooks.md) for a hierarchical structure

## Comparison with Workflowy

| Feature | Joplin | Workflowy |
|---------|--------|-----------|
| Nested lists | ✓ Yes (via markdown indentation) | ✓ Yes |
| Keyboard shortcuts for indent/outdent | ✓ Yes | ✓ Yes |
| Checkboxes | ✓ Yes | ✓ Yes (via tags) |
| Collapse/expand items | Headings only | ✓ Yes (all items) |
| Zoom into items | No (use separate notes) | ✓ Yes |
| Offline access | ✓ Yes | Premium only |
| Formatting | ✓ Full Markdown | Limited |
| Images and attachments | ✓ Yes | Limited |

## Example: Meeting Notes Outline

Here's a practical example of using Joplin for meeting notes:

```markdown
# Team Meeting - 2024-02-01

## Attendees
- Alice (Project Manager)
- Bob (Developer)
- Carol (Designer)

## Agenda
1. Project status update
    - [x] Backend API
        - All endpoints complete
        - Documentation in progress
    - [ ] Frontend UI
        - 80% complete
        - Need review on color scheme
    - [ ] Testing
        - Unit tests done
        - Integration tests pending
2. Upcoming milestones
    - Feb 15: Beta release
    - Mar 1: User feedback review
    - Mar 15: Production release
3. Action items
    - [ ] Bob: Complete API documentation by Feb 5
    - [ ] Carol: Share design mockups by Feb 3
    - [ ] Alice: Schedule user testing sessions

## Notes
- Consider adding dark mode
- Need to discuss mobile responsiveness
    - iPhone testing required
    - Android testing required
```

## Tips for Converting from Workflowy

If you're coming from Workflowy:

1. **Export from Workflowy**: Export your outlines as plain text or OPML
2. **Convert to Markdown**: Use `- ` for each list item and indent with tabs or spaces
3. **Import to Joplin**: Paste directly into a new note or import via the import feature
4. **Adjust workflow**: Get familiar with using headings for major sections and consider splitting very large outlines into multiple linked notes

## Related Features

- [Markdown Guide](https://github.com/laurent22/joplin/blob/dev/readme/apps/markdown.md) - Full markdown syntax reference
- [To-dos](https://github.com/laurent22/joplin/blob/dev/readme/apps/to-dos.md) - Using Joplin for task management
- [Link to Note](https://github.com/laurent22/joplin/blob/dev/readme/apps/link_to_note.md) - Connecting related notes
- [Subnotebooks](https://github.com/laurent22/joplin/blob/dev/readme/apps/subnotebooks.md) - Organizing notes hierarchically
