- Project Title
	- [[RNAseq]] Literature Review: Pre/Post [[Radiation Therapy]] in [[Cancer]]
- Objective
	- Main objective: Identify differential gene expression datasets comparing before and after radiation therapy
	- Identify studies with [[RNAseq]] data collected before AND after radiation monotherapy
	- Contact authors to request raw data for downstream analysis
- Inclusion Criteria
	- Human subjects
	  logseq.order-list-type:: number
	- Radiation monotherapy only (no chemo/immunotherapy combo)
	  logseq.order-list-type:: number
	- [[RNAseq]] performed at minimum 2 timepoints: pre-RT and post-RT
	  logseq.order-list-type:: number
	- [[DEG analysis]] performed or raw counts available
	  logseq.order-list-type:: number
	- Any [[cancer]] type
	  logseq.order-list-type:: number
- Exclusion Criteria
	- Animal/cell line studies
	  logseq.order-list-type:: number
	- Combined treatment modalities
	  logseq.order-list-type:: number
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
- Deliverables
	- Logseq pages per paper with attributes
	  logseq.order-list-type:: number
	- Queryable graph via tags/attributes
	  logseq.order-list-type:: number