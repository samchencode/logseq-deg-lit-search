- Project Title
	- [[RNAseq]] Literature Review: Pre/Post [[Radiation Therapy]] in [[Cancer]]
- Objective
	- Main objective: Identify differential gene expression datasets comparing before and after radiation therapy
	- Identify studies with [[RNAseq]] data collected before AND after radiation monotherapy
	- Contact authors to request raw data for downstream analysis
- Inclusion Criteria
	- Human subjects or patient derived xenograft
	- Radiation monotherapy only (no chemo/immunotherapy combo)
	- [[RNAseq]] performed at minimum 2 timepoints: pre-RT and post-RT (bulk RNAseq OR scRNA-seq)
	- [[DEG analysis]] performed or raw counts available
	- Any [[cancer]] type
	- Review/meta-analysis articles using RNAseq methods are acceptable (may reference other papers that fit search criteria)
- Exclusion Criteria
	- Animal/cell line studies
	- Combined treatment modalities
	- Non-transcriptomics methods (e.g., DNA methylation, proteomics, metabolomics) - studies must use transcriptomics (RNAseq) methodology
- Partial Data Handling
	- Papers with only pre-RT or post-RT = tagged `partial-data`
	- Missing fields = NA
- Data Extraction Schema (page attributes)
	- `tags::` paper (add partial-data if applicable)
	- `link::` [LINK](url)
	- `authors::` Last, F et al
	- `n::` patient count or NA
	- `dose-cgy::` radiation dose or NA
	- `time-post-rt::` days post-RT or NA
	- `disease-site::` cancer type
	- `pub-date::` YYYY-MM-DD or NA
	- `tissue-pre-rt::` tissue type before RT
	- `tissue-post-rt::` tissue type after RT
	- `fractionation::` number of fractions or NA
	- `deg-comparison::` paired pre/post same patient, control vs post-RT, or NA
- Storage
	- Filename: `pages/<doi>.md` (replace `/` with `_`)
	- Deduplication: DOI as filename prevents duplicates
	- Sample size: >1, no upper limit
- Search Strategy
	- Primary: [[PubMed]] (Claude searchable)
	- Secondary: [[Scopus]], [[Semantic Scholar]], [[Consensus AI]], [[Perplexity]] (paste results)
	- Keywords: RNAseq, RNA-seq, transcriptome, radiation, radiotherapy, differential expression, pre post
- Public Data Check
	- Before contacting authors, check [[Public Data Sources]]
- Search Tracking Workflow
	- Each retrieval logged in daily journal under `journals/yyyy_MM_dd.md`
	- Format:
	  ```
	  - Search N
	  	- [[doi_here]] - brief synopsis
	  	- [[doi_here]] - brief synopsis
	  ```
	- Searches numbered sequentially per day (Search 1, Search 2, etc.)
	- Each paper DOI linked creates backlink to journal date
	- Enables tracking what was found when
- Manual Search Workflow
	- Failed article retrievals (blocked bots, 403, paywall, file too large, network failure)
	- Log to `pages/Manual Search.md`:
	  ```
	  - <date/time> - article title
	  	- DOI: <doi>
	  	- Link: [source](url)
	  	- Issue: <reason for failure>
	  ```
- Deliverables
	- Logseq pages per paper with attributes
	  logseq.order-list-type:: number
	- Queryable graph via tags/attributes
	  logseq.order-list-type:: number
	- Journal log of all searches
	  logseq.order-list-type:: number