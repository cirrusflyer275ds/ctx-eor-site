# Recruiting Data Strategy: Source Documentation and Weighting Rationale

This README documents the core public datasets leveraged by the Hireway Recruiting Intelligence Engine. It explains the purpose of each dataset, how it's used, and its relative weight in generating smart, tailored recruiting outputs including ad copy, placement strategy, targeting insights, and qualification scoring.

---

## Purpose of This File

This file exists to:

* Clarify which public datasets are being used.
* Explain how each data source connects to our recruiting workflows.
* Document the relative **weights** used in scoring and prioritization.
* Support transparency, reproducibility, and future refinement.

---

## Primary Data Sources and Rationale

### 1. **O\*NET (Occupational Information Network)**

* **Use:** Job-specific knowledge, skills, abilities, personality traits, experience levels, and task descriptions.
* **Why:** O\*NET is the most comprehensive role-level occupational dataset in the U.S. and forms the semantic foundation for role understanding.
* **Weight:** **40%**
* **Notes:** Anchors all job-related modeling. Mapped to SOC codes. Used for both recruiting copy tone and interview logic.

---

### 2. **NAICS (North American Industry Classification System)**

* **Use:** Understand the employer's industry context.
* **Why:** Helps tailor tone, expectations, ad placement channels, and messaging to industry norms and jargon.
* **Weight:** **10%**
* **Notes:** Used to infer expected education, terminology, and messaging style. May adjust visuals or reference materials.

---

### 3. **BLS OES Industry-Occupation Matrix**

* **Use:** Crosswalk between NAICS and SOC codes, includes employment density by industry.
* **Why:** Supports mapping from company type to likely needed occupations. Supports ad targeting strategy.
* **Weight:** **10%**
* **Notes:** Used in building recommended roles per industry and headcount estimates.

---

### 4. **U.S. Census Demographic Data (County, MSA, ZIP-level)**

* **Use:** Population density, income bands, education attainment, languages spoken.
* **Why:** Critical for geo-targeting and modifying ad copy for accessibility or appeal.
* **Weight:** **15%**
* **Notes:** Used to shape inclusive ad language and outreach tone. Also informs what platforms are viable.

---

### 5. **State Department of Labor Job Postings + Wage Data**

* **Use:** Real-time job posting trends, salary ranges by state or metro.
* **Why:** Enhances regional realism in job descriptions, ensures competitiveness.
* **Weight:** **10%**
* **Notes:** Data quality varies by state. Used to benchmark ad competitiveness.

---

### 6. **Bureau of Labor Statistics (BLS) National + Local**

* **Use:** Unemployment rates, occupation growth trends, labor participation.
* **Why:** Supports understanding of talent supply constraints and urgency messaging.
* **Weight:** **5%**

---

### 7. **Internal CTX-EOR Benchmarks** *(Future)*

* **Use:** Real hiring success, trial conversion, and screening data.
* **Why:** Eventually replaces or calibrates public data with private insight.
* **Weight:** N/A (future)

---

## Output Applications

* **Ad Copy Generator**: Adjusts tone, reading level, keywords, benefits emphasis.
* **Ad Platform Suggestion**: Based on geo-demographics + job type.
* **Minimum Qualification Screening**: Based on O\*NET traits + geography.
* **Candidate Scoring & Prioritization**: Merges resume data + external benchmarks.

---

## Next Steps

* Build version-controlled modules to ingest and update each dataset.
* Track how weights perform and adjust based on trial outcomes.
* Allow customers to tweak emphasis using a visual weighting interface.

---

This README is essential for ongoing technical transparency and performance evaluation as Hireway's smart recruiting product grows.
