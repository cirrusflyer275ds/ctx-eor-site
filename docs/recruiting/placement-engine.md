# Placement Engine

This module outlines how CTX-EOR automatically recommends and manages job ad placements for customers based on role type, geography, budget, and campaign strategy.

---

## Purpose

The Placement Engine ensures that job postings are:

* **Strategically distributed** across platforms best suited to the role
* **Optimized for geography** and expected applicant behavior
* **Budget-conscious** based on customer input or recommended tiers
* **Evolving** with trends in platform performance by role and industry

---

## Core Inputs

1. **Role Type**

   * SOC Code
   * Title and description
   * Shift type (e.g. day/night/weekend)

2. **Industry Context**

   * NAICS code
   * Common hiring channels for industry

3. **Geographic Location**

   * Zip code / metro area
   * Rural, urban, or suburban targeting logic

4. **Budget Level**

   * Customer-defined or defaulted tier (e.g., \$100, \$500, \$1000+)

5. **Employer Voice Preferences** (optional)

   * Culture-forward vs. benefit-driven vs. high-urgency

---

## Output: Platform Plan

The system will generate a platform distribution plan such as:

| Platform      | Budget % | Ad Style         | Justification                            |
| ------------- | -------- | ---------------- | ---------------------------------------- |
| Facebook Jobs | 40%      | Short-form + CTA | High local reach, strong blue-collar ROI |
| Craigslist    | 30%      | Direct, bold     | Targeting low-cost seekers               |
| ZipRecruiter  | 20%      | Hybrid style     | Resume-focused searchers                 |
| Google Jobs   | 10%      | SEO-optimized    | Organic candidate inflow                 |

---

## Ruleset Examples

* **If job = software engineer + urban = true →** Prioritize LinkedIn + AngelList
* **If job = warehouse + rural = true →** Craigslist + Facebook local
* **If industry = healthcare →** Add niche boards like HealthJobs.com

---

## Customer UI Preview (Planned)

* Checkbox toggles for each proposed platform
* Editable budget per platform
* "Why this platform?" tooltips
* Auto-preview of ad format per channel

---

## Future Enhancements

* Campaign A/B testing logic
* Predictive ad duration suggestions
* Feedback loop from Campaign Viewer

---

> This engine forms the foundation of CTX-EOR’s data-driven recruiting service. By connecting job attributes, geography, and platform logic, it ensures smarter budget use and better hiring outcomes.

---

File location: `docs/recruiting/placement-engine.md`
