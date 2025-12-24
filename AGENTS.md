# Agent Instructions

Be concise, sacrifice grammar for brevity. Minimize file redundancy.

## Project

Logseq graph for literature review. Key docs:
- `pages/Planning.md` - plan & milestones
- `pages/Project Specification.md` - finalized requirements
- `pages/Tips.md` - search patterns & lessons learned

## Directories

- **journals/**: Daily journal pages (auto-created by Logseq)
- **pages/**: User-created titled pages
- **assets/**: Images, PDFs, media

## Naming

Journal: `yyyy_MM_dd.md` (e.g., `2025_12_23.md`)
Pages: Use title as filename, preserve spaces/caps (e.g., `My Page.md`)
Paper pages: `pages/<doi>.md` (replace `/` with `_` in DOI)

## Links

Wrap nouns in `[[ ]]` (e.g., `[[The concept]]`), create corresponding page file in `pages/`

## Page Attributes

Top of file: `key:: value`. See `pages/Example Paper.md`.

Required for papers:
```
tags:: paper
link:: [LINK](url)
authors:: Last, F et al
n:: patient count or NA
dose-cgy:: dose or NA
time-post-rt:: days or NA
disease-site:: cancer type
pub-date:: YYYY-MM-DD or NA
tissue-pre-rt:: tissue type before RT
tissue-post-rt:: tissue type after RT
fractionation:: number of fractions or NA
deg-comparison:: paired pre/post same patient, control vs post-RT, or NA
```
Partial data (only pre-RT or post-RT): add `partial-data` to tags

## Search Tracking

In daily journal (`journals/yyyy_MM_dd.md`):
```
- Search N
	- [[doi_here]] - brief synopsis
	- [[doi_here]] - brief synopsis
```
Add to search log immediately when matching paper found, create `pages/<doi>.md` with attributes.

## Workflow

Always create todo list and check off as you go.
