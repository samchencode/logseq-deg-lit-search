- What is the goal of this project?
  logseq.order-list-type:: number
	- Find papers with [[RNAseq]] data before AND after [[radiation therapy]] for [[cancer]] (any type)
	  logseq.order-list-type:: number
	- Gather contact info to request raw data for own study
	  logseq.order-list-type:: number
- Inclusion Criteria
  logseq.order-list-type:: number
	- Human subjects only
	  logseq.order-list-type:: number
	- Radiation monotherapy (no combo with chemo/immunotherapy)
	  logseq.order-list-type:: number
	- RNAseq performed pre-RT AND post-RT
	  logseq.order-list-type:: number
	- [[DEG analysis]] context
	  logseq.order-list-type:: number
- Data Schema (per paper)
  logseq.order-list-type:: number
	- Author
	  logseq.order-list-type:: number
	- Full text link
	  logseq.order-list-type:: number
	- Patient count
	  logseq.order-list-type:: number
	- Radiation dose (cGy)
	  logseq.order-list-type:: number
	- Days post-RT for sample collection
	  logseq.order-list-type:: number
- Search Sources
  logseq.order-list-type:: number
	- [[PubMed]] - searchable via Claude
	  logseq.order-list-type:: number
	- [[Scopus]] - paste results for processing
	  logseq.order-list-type:: number
	- [[Semantic Scholar]] / [[Consensus AI]] / [[Perplexity]] - paste results
	  logseq.order-list-type:: number
- Storage
  logseq.order-list-type:: number
	- Each paper = `pages/<doi>.md` (replace `/` with `_`)
	  logseq.order-list-type:: number
	- Data stored as Logseq page attributes (see [[Example Paper]])
	  logseq.order-list-type:: number
	- Deduplication via DOI filename
	  logseq.order-list-type:: number
- Missing Data Handling
  logseq.order-list-type:: number
	- Missing fields = NA
	  logseq.order-list-type:: number
	- Partial data (pre-RT only or post-RT only) = add `partial-data` to tags
	  logseq.order-list-type:: number
- Sample Size
  logseq.order-list-type:: number
	- Minimum: >1 paper
	  logseq.order-list-type:: number
	- No upper limit
	  logseq.order-list-type:: number
- Public Data Sources
  logseq.order-list-type:: number
	- Check [[Public Data Sources]] before contacting authors
	  logseq.order-list-type:: number
- What are the milestones?
  logseq.order-list-type:: number
	- Phase 1: Acquisition. Search databases, paste results for processing
	  logseq.order-list-type:: number
	- Phase 2: Verification. Filter for inclusion criteria, check public data
	  logseq.order-list-type:: number
	- Phase 3: Aggregation. Create paper pages with attributes
	  logseq.order-list-type:: number
- ### Background information
	- Example Data Source Paper
		- Response to Preoperative Radiation Therapy in Relation to Gene Expression Patterns in Breast Cancer Patients
			- Development and validation of a novel radiosensitivity signature in human breast cancer
	- About CURE AI
		- [A Deep Learning Framework for Causal Inference in Clinical Trial Design: The CURE AI Large Clinicogenomic Foundation Model](https://www.medrxiv.org/content/10.1101/2025.03.06.25323534v1)
		- [Artificial intelligence in target discovery: CURE AI prediction of TIGIT and PD-L1 as immunotherapy targets in NSCLC](https://ascopubs.org/doi/10.1200/JCO.2025.43.16_suppl.e13692)
	- We also have 10 PDX lines