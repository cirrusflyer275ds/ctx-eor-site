# Ad Copy Generator

This module outlines how CTX-EOR generates recruiting ad copy tailored to the job, company, and location—using structured data and AI-driven personalization.

---

## Objective

To create high-performing, job-specific advertisements that reflect the role, industry, and company culture using structured inputs and LLM-generated variations.

---

## Inputs Required

- SOC Code / Job Title
- NAICS Code (Industry)
- Location (City, ZIP, or Region)
- Work Environment (e.g., office, warehouse, outdoors)
- Schedule & Pay Information
- Experience Level and Education Requirements
- Any unique selling points (e.g., bonuses, benefits)

---

## Strategy

- Use O*NET attributes to describe the nature of the work
- Adjust language based on the target candidate profile (tone, formality, emphasis on mission or benefits)
- Use AI to vary tone based on:
  - Job category (blue-collar, grey-collar, white-collar)
  - Company size and employer brand (startup vs. established)
  - Geographic norms (urban, rural)

---

## Output

Multiple versions of job ads including:

- Short-form (for SMS or quick previews)
- Long-form (for full job postings)
- Social-formatted (for platforms like Facebook or Instagram)

Each version includes:

- Headline
- Summary paragraph
- Role expectations
- Perks and employer pitch
- Application CTA

---

> This is a scaffold only. The logic for the tone engine and variant generation will be handled by an LLM prompt pipeline.

