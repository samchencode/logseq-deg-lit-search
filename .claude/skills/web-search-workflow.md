---
description: Execute the literature search workflow for finding radiation therapy DEG papers
---

# Web Search Workflow

Execute the literature search workflow for this Logseq graph.

## Instructions

Before starting or continuing, review `pages/Project Specification.md` to refresh on instructions and check `pages/Search History.md` for previously used search terms to avoid repetition.

### Search Tracking Format

When matching paper found, add to daily journal (`journals/yyyy_MM_dd.md`) immediately:
```
- Search N
	- [[doi_here]] - brief synopsis
	- [[doi_here]] - brief synopsis
```

Create `pages/<doi>.md` with required attributes (see CLAUDE.md Page Attributes section).

### Manual Search Tracking

Failed article retrievals (blocked bots, 403, paywall, file too large, network failure) go to `pages/Manual Search.md`:
```
- <date/time> - article title
	- DOI: <doi>
	- Link: [source](url)
	- Issue: <reason for failure>
```

### Workflow Steps

1. Search for articles
2. Found article?
   - Yes: Stop searching and update daily journal + make page for found article
   - No: Continue searching
3. Add failed article retrievals to `pages/Manual Search.md` per format above
4. Update `pages/Search History.md` - add all used search terms this run
5. Update `pages/Tips.md` with tips for finding best articles
6. Stop and wait for instructions to continue the search

Always create todo list and check off as you go.
