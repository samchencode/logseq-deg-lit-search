# CLAUDE.md

In all interactions and commit messages, be extremely concise and sacrifice grammar for the sake of being concise.

## Project Overview

This is a Logseq graph for a literature review project. Key docs:
- `pages/Planning.md` - project plan and milestones
- `pages/Project Specification.md` - finalized requirements

## Directory Structure

### Core Directories

- **journals/**: Daily journal pages created automatically by Logseq. Each day you open Logseq, a new journal page is created. This is where you typically start writing notes before organizing them into dedicated pages.

- **pages/**: User-created titled pages for organizing knowledge. Notes that start in journal pages are often moved here as they develop into distinct topics.

- **assets/**: Storage for images, PDFs, and other media files referenced in your notes.

## Naming Conventions

### Journal Files
- Journal files are named by date in `yyyy_MM_dd.md` format (e.g., `2025_12_23.md`)
- Journal file naming format can be customized in Logseq settings to include additional information like day of week
- Alternative formats may create hierarchical namespacing for month and year pages

### Page Files
- Page files use the page title as the filename with `.md` extension
- Spaces in page titles become spaces in filenames (e.g., "My Page" → `My Page.md`)
- Special characters and capitalization in page names should be preserved in filenames
- Namespacing is supported using `/` in page names (e.g., "Project/Notes" creates hierarchy)

## Linking Rules

When writing markdown files, wrap nouns in `[[ ]]` (e.g., `[[The concept]]`) and create corresponding page file in `pages/` (e.g., `pages/The concept.md`).

## Page Attributes

Logseq page attributes go at top of file, format `key:: value`. See `pages/Example Paper.md`. Paper pages use DOI as filename: `pages/<doi>.md` (replace `/` with `_` in DOI).

Required attributes for papers:
```
tags:: paper
link:: [LINK](url)
authors:: Last, F et al
n:: patient count or NA
dose-cgy:: dose or NA
time-post-rt:: days or NA
disease-site:: cancer type
```

For partial data (only pre-RT or post-RT), add `partial-data` to tags.

## Workflow

The recommended Logseq workflow:
1. Start by writing notes in daily journal pages
2. As ideas develop, create dedicated pages and move/link content from journals
3. Use bi-directional links `[[Page Name]]` to connect related concepts
4. Build a knowledge graph through consistent linking and organization
