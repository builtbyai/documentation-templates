# Obsidian Callouts Template

**Purpose**: Complete reference for Obsidian callout syntax
**Source**: Compiled from 6 Obsidian vault templates
**Usage**: Use callouts to highlight important information in your notes

---

## Table of Contents
1. [Basic Callouts](#basic-callouts)
2. [Collapsible Callouts](#collapsible-callouts)
3. [Nested Callouts](#nested-callouts)
4. [Custom Titles](#custom-titles)
5. [All Callout Types](#all-callout-types)

---

## Basic Callouts

### Info Callout
```markdown
> [!info]
> This is an informational callout. Use it to provide helpful context or explanations.
```

**Result**:
> [!info]
> This is an informational callout. Use it to provide helpful context or explanations.

### Tip Callout
```markdown
> [!tip]
> This is a tip callout. Share pro tips, shortcuts, or best practices here.
```

**Result**:
> [!tip]
> This is a tip callout. Share pro tips, shortcuts, or best practices here.

### Note Callout
```markdown
> [!note]
> This is a note callout. Use it for general notes or observations.
```

**Result**:
> [!note]
> This is a note callout. Use it for general notes or observations.

### Warning Callout
```markdown
> [!warning]
> This is a warning callout. Alert users to potential issues or important considerations.
```

**Result**:
> [!warning]
> This is a warning callout. Alert users to potential issues or important considerations.

### Success Callout
```markdown
> [!success]
> This is a success callout. Celebrate achievements or confirmed positive outcomes.
```

**Result**:
> [!success]
> This is a success callout. Celebrate achievements or confirmed positive outcomes.

### Error/Danger Callout
```markdown
> [!error]
> This is an error callout. Highlight critical issues or things to avoid.
```

**Result**:
> [!error]
> This is an error callout. Highlight critical issues or things to avoid.

---

## Collapsible Callouts

### Collapsed by Default (-)
```markdown
> [!info]- Click to expand
> This content is hidden by default. Click the arrow to reveal it.
>
> You can include multiple paragraphs, lists, code blocks, and more.
```

**Result**:
> [!info]- Click to expand
> This content is hidden by default. Click the arrow to reveal it.
>
> You can include multiple paragraphs, lists, code blocks, and more.

### Expanded by Default (+)
```markdown
> [!tip]+ Expanded by default
> This content is visible by default but can be collapsed.
>
> - List item 1
> - List item 2
> - List item 3
```

**Result**:
> [!tip]+ Expanded by default
> This content is visible by default but can be collapsed.
>
> - List item 1
> - List item 2
> - List item 3

---

## Nested Callouts

### Callout Inside Callout
```markdown
> [!info] Main Information
> This is the outer callout with important information.
>
> > [!warning] Nested Warning
> > This is a nested callout inside the info callout.
> > Use nested callouts to show hierarchical information.
>
> Back to the main info callout content.
```

**Result**:
> [!info] Main Information
> This is the outer callout with important information.
>
> > [!warning] Nested Warning
> > This is a nested callout inside the info callout.
> > Use nested callouts to show hierarchical information.
>
> Back to the main info callout content.

### Multi-Level Nesting
```markdown
> [!note] Level 1
> First level callout
>
> > [!tip] Level 2
> > Second level callout
> >
> > > [!success] Level 3
> > > Third level callout - use sparingly!
```

**Result**:
> [!note] Level 1
> First level callout
>
> > [!tip] Level 2
> > Second level callout
> >
> > > [!success] Level 3
> > > Third level callout - use sparingly!

---

## Custom Titles

### Custom Title with Info
```markdown
> [!info] Custom Title Here
> You can customize the title of any callout type.
> This makes it more specific to your content.
```

**Result**:
> [!info] Custom Title Here
> You can customize the title of any callout type.
> This makes it more specific to your content.

### Custom Title with Collapsible
```markdown
> [!warning]- Important Security Considerations
> This collapsible callout has a custom title.
> Click to expand and see the security guidelines.
>
> 1. Always validate user input
> 2. Use parameterized queries
> 3. Implement proper authentication
```

**Result**:
> [!warning]- Important Security Considerations
> This collapsible callout has a custom title.
> Click to expand and see the security guidelines.
>
> 1. Always validate user input
> 2. Use parameterized queries
> 3. Implement proper authentication

---

## All Callout Types

### Complete Reference

#### [!note] - General Notes
```markdown
> [!note]
> Default callout for general notes and observations.
```

#### [!abstract] / [!summary] / [!tldr]
```markdown
> [!abstract]
> Summarize key points or provide an overview.
```

#### [!info] / [!todo]
```markdown
> [!info]
> Provide helpful information or context.
```

#### [!tip] / [!hint] / [!important]
```markdown
> [!tip]
> Share helpful tips, shortcuts, or best practices.
```

#### [!success] / [!check] / [!done]
```markdown
> [!success]
> Indicate successful completion or positive outcomes.
```

#### [!question] / [!help] / [!faq]
```markdown
> [!question]
> Pose questions or provide FAQ content.
```

#### [!warning] / [!caution] / [!attention]
```markdown
> [!warning]
> Alert users to potential issues or important considerations.
```

#### [!failure] / [!fail] / [!missing]
```markdown
> [!failure]
> Indicate failures, missing items, or incomplete tasks.
```

#### [!error] / [!danger]
```markdown
> [!error]
> Highlight critical errors or dangerous situations.
```

#### [!bug]
```markdown
> [!bug]
> Document bugs or issues that need fixing.
```

#### [!example]
```markdown
> [!example]
> Provide examples or demonstrations.
```

#### [!quote] / [!cite]
```markdown
> [!quote]
> Include quotations or cited material.
```

---

## Advanced Usage Examples

### Documentation Section
```markdown
> [!info]+ API Documentation
> # User Authentication Endpoint
>
> **URL**: `/api/auth/login`
> **Method**: POST
>
> **Request Body**:
> ```json
> {
>   "username": "string",
>   "password": "string"
> }
> ```
>
> **Response**:
> ```json
> {
>   "token": "jwt_token_here",
>   "expires": "2024-12-31T23:59:59Z"
> }
> ```
```

### Troubleshooting Guide
```markdown
> [!bug]- Login Issues
> If users cannot log in, check the following:
>
> > [!question] Is the database accessible?
> > Verify database connection settings in `.env` file.
>
> > [!question] Are credentials correct?
> > Check username/password hash in database.
>
> > [!tip] Common Fix
> > Clear browser cache and cookies, then try again.
```

### Project Checklist
```markdown
> [!todo]+ Project Tasks
> - [x] Requirements gathering
> - [x] Design mockups
> - [ ] Backend development
>   - [x] Database schema
>   - [ ] API endpoints
>   - [ ] Authentication
> - [ ] Frontend development
> - [ ] Testing
> - [ ] Deployment
>
> > [!warning] Deadline
> > Project must be completed by December 31, 2024
```

### Code Example with Explanation
```markdown
> [!example]+ React Component Example
> ```jsx
> function UserProfile({ user }) {
>   return (
>     <div className="profile">
>       <h2>{user.name}</h2>
>       <p>{user.email}</p>
>     </div>
>   );
> }
> ```
>
> > [!tip] Best Practice
> > Always destructure props for cleaner, more readable code.
>
> > [!warning] Common Mistake
> > Don't forget to add PropTypes validation for type safety.
```

---

## Best Practices

### When to Use Each Callout Type

**[!info]** - Contextual information that enhances understanding
- Background information
- Definitions
- Related concepts

**[!tip]** - Actionable advice that improves workflow
- Shortcuts
- Best practices
- Pro tips
- Performance optimizations

**[!warning]** - Important considerations that could cause issues
- Breaking changes
- Deprecated features
- Gotchas
- Performance concerns

**[!error]** - Critical information to prevent mistakes
- Security vulnerabilities
- Data loss scenarios
- Destructive operations

**[!success]** - Positive confirmations and achievements
- Successful completion
- Validation passed
- Goals achieved

**[!note]** - General observations and supplementary information
- Additional details
- Side notes
- Clarifications

### Styling Tips

1. **Keep Titles Concise**: Use 2-5 words for custom titles
2. **Use Collapsible for Long Content**: Anything over 5 lines should be collapsible
3. **Nest Sparingly**: Avoid more than 2 levels of nesting
4. **Be Consistent**: Use the same callout types for similar content across your vault
5. **Don't Overuse**: Too many callouts reduce their impact - use strategically

### Content Organization

```markdown
> [!abstract]+ Document Overview
> High-level summary at the top

## Main Content Section

Regular markdown content goes here...

> [!tip] Inline Tips
> Scattered throughout where relevant

## Technical Details

> [!example]- Code Examples
> Detailed examples in collapsible sections

> [!warning] Important Caveats
> Critical warnings where needed

## Summary

> [!success] Key Takeaways
> Summarize learnings at the end
```

---

## Callout Color Reference

| Type | Color | Common Aliases |
|------|-------|----------------|
| note | Blue | - |
| abstract | Cyan | summary, tldr |
| info | Blue | todo |
| tip | Green | hint, important |
| success | Green | check, done |
| question | Orange | help, faq |
| warning | Orange | caution, attention |
| failure | Red | fail, missing |
| error | Red | danger |
| bug | Red | - |
| example | Purple | - |
| quote | Gray | cite |

---

## Markdown in Callouts

### Supported Markdown Elements

Callouts support all standard markdown syntax:

```markdown
> [!info]+ Full Markdown Support
>
> # Headers work
> ## At all levels
>
> **Bold** and *italic* text
>
> - Unordered lists
> - Work perfectly
>
> 1. Ordered lists
> 2. Also supported
>
> `Inline code` and code blocks:
> ```python
> def hello():
>     print("Hello from callout!")
> ```
>
> [Links](https://example.com) and [[Internal Links]]
>
> ![Images](image.png)
>
> > Regular blockquotes
> > Still work inside
>
> | Tables | Also |
> |--------|------|
> | Work   | Fine |
```

---

**Template Version**: 1.0
**Last Updated**: 2025-12-28
**Obsidian Version**: Compatible with v1.0+
**Source Files**: 6 Obsidian markdown templates
