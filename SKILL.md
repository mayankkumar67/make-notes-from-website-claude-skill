---
name: make-notes
description: "Read the current web page and save to Notion with key points, code, diagrams, and technical analysis for experienced frontend developers. Can create new pages or append to existing ones."
---

# Make Notes

Captures web page content tailored for experienced frontend developers (5+ years). Focuses on architectural decisions, performance implications, gotchas, and practical integration patterns—not basic concepts.

## What gets extracted

- **Key Technical Points** – architectural decisions, design patterns, performance implications, browser/framework compatibility
- **Important Terminology** – only non-obvious terms; assumes knowledge of standard FE concepts (DOM, events, async/await, etc.)
- **Code Analysis** – code examples with comments on performance, best practices, potential issues, and modern alternatives
- **Diagrams & Visuals** – architecture diagrams, performance charts, flow diagrams
- **Gotchas & Edge Cases** – common pitfalls, browser quirks, version incompatibilities, antipatterns to avoid
- **Integration Notes** – how it fits with modern tooling (webpack, Vite, TypeScript, React, Vue, etc.)

## How it works

1. **Parse the page**: Extracts content using Claude in Chrome
2. **Technical analysis**: Identifies architectural patterns, performance considerations, and compatibility notes
3. **Extract code**: Pulls code blocks with analysis of what matters (efficiency, compatibility, edge cases)
4. **Capture visuals**: Screenshots of relevant diagrams and charts
5. **Save to Notion**: Creates a new page OR appends to an existing page

## Usage Modes

### Create New Page (Default)
Simply say:
- "Make notes on this page"
- "Capture this article to Notion"
- "Save technical notes"

Creates a new page in your Notion workspace.

### Append to Existing Page
Share the Notion page with Claude and say:
- "Add notes from this page to my [page name] in Notion"
- "Append these notes to my React notes page"
- "Save to my existing web clippings page"

Appends the extracted content to your existing page without deleting anything.

## Notion page structure

**Source**: [URL] | **Published**: [Date]

### Key Technical Points
- Pattern/Decision: [Analysis of why this approach, tradeoffs, performance impact]
- Browser Compatibility: [Which versions, known issues]
- Performance Consideration: [Implications, metrics if available]

### Important Concepts
- **Term**: [Why it matters, when/how to use, gotchas]
- **Pattern Name**: [When to apply, alternative approaches, when not to use]

### Code Examples & Analysis
```javascript
// Code with inline notes on:
// - Performance implications
// - Browser compatibility
// - Modern alternatives
// - Potential issues
```

### Gotchas & Edge Cases
- [Known issue + workaround]
- [Browser quirk + detection/handling]
- [Common mistake + solution]

### Integration Notes
- Tooling: webpack/Vite/other implications
- Framework compatibility (React/Vue/Svelte/etc.)
- Dependency requirements and versions
- Breaking changes vs. previous versions

### Diagrams & Architecture
[Visual representations with annotations]

### Quick Reference
[TL;DR summary with key metrics/benchmarks if available]

## Organizing Multiple Sources

### Option 1: Append to One Master Page
Keep all notes in a single "Web Clippings" or "Learning" page:
- "Append notes to my learning page"
- Organizes everything in one searchable location
- Use Notion page properties (tags, source URL) to categorize

### Option 2: Use Notion Databases
Create a Notion database with articles as entries:
- Each new note becomes a database entry
- Filter and sort by topic, date, framework, etc.
- Link related entries together
- Create rollups to see key concepts across articles

### Option 3: Topic-Specific Pages
Maintain separate pages for each topic:
- "React notes page" for React articles
- "Performance notes page" for optimization articles
- "TypeScript notes page" for TypeScript resources
- Append to the relevant page based on topic

## What to say

**New page:**
- "Make notes on this page"
- "Capture this FE article/docs"
- "Make technical notes on this page"
- "Save with dev-level analysis"

**Append to existing:**
- "Add these notes to my [page name]"
- "Append to my web clippings"
- "Add to my React learning page"
- "Save to my existing notes"

## What it skips

- Basic JavaScript/CSS/HTML explanations
- Simple term definitions that experienced devs would know
- Beginner-level concepts
- Generic tutorials without technical depth

## Best for

- Technical blog posts and deep dives
- Framework/library documentation
- Performance optimization guides
- Architecture pattern articles
- Best practices and patterns
- Tool configuration guides
- RFCs and technical specs

## Tips for Appending

✅ **Works great:**
- Appending to a database entry
- Adding new sections to an existing page
- Building a knowledge base over time
- Keeping related resources in one place

⚠️ **Tips:**
- Share the Notion page with Claude (in the prompt or use link sharing)
- Use consistent page names so Claude knows where to save
- Tag or categorize appended notes so they're easy to find
- Review appended content – you can always clean up formatting in Notion
