# Ad Copy Generator

This module outlines how Hireway generates high-conversion recruiting advertisements tailored to the role, company, and location—powered by structured data and AI-driven personalization.

---

## Purpose

Hireway’s Ad Copy Generator is designed to:

- Automate job ad creation using role-specific data
- Reflect the employer’s tone and priorities
- Customize messaging based on geography, industry, and demographics
- Deliver copy variants tailored to different advertising platforms

---

## Inputs

The generator uses a combination of structured inputs to define the ad:

1. **SOC Code**
   - Informs duties, environment, core skills, and work activities
2. **NAICS Code**
   - Adds industry framing and employer-type phrasing
3. **Location Data**
   - Zip code, city, or metro for regional idioms, transportation tips, wage expectations
4. **Demographics**
   - Uses Census and labor data to match tone and call-to-action strength with candidate profiles
5. **Customer Preferences**
   - Options like casual vs. formal, urgency vs. opportunity, benefit vs. culture-forward
6. **Trial Configuration**
   - Schedule, pay, expectations, entry requirements (experience/education)
7. **Work Environment**
   - Office, warehouse, outdoors, field service, etc.

---

## Output

Hireway produces multiple ad formats:

| Format         | Use Case                    | Example Use         |
|----------------|-----------------------------|----------------------|
| **Short Ad**   | Craigslist, SMS              | “Hiring now: Entry-level warehouse role. Great team. Apply today.” |
| **Medium Ad**  | Facebook, Instagram          | “Join a fast-growing logistics team in your city. Great pay, no experience required. Paid training and growth ahead.” |
| **Long Ad**    | ZipRecruiter, Indeed, Email  | Full breakdown including role summary, expectations, perks, and application CTA |
| **Narrative**  | Email outreach, job site blog| Company mission + team culture + job specifics, with warm tone |

Each version is:
- **Editable** via the Customization Panel
- **Version-tracked** so customers can revert or branch
- **Auto-tagged** by tone, format, and platform

---

## Style & Tone Logic

The generator adapts tone using AI prompt logic:

- **By job category** (blue/grey/white collar)
- **By company type** (startup, local biz, enterprise)
- **By urgency** (e.g., “start Monday” vs. “grow with us”)
- **By geography** (urban formality vs. rural clarity)

Customers can override tone settings through the **Customization Panel** (see linked module).

---

## Example Ad Versions (Warehouse Associate in Chicago)

**Short:**
> “Hiring Warehouse Team Member – $17/hr + growth! Day shift, paid training. Apply now.”

**Medium:**
> “Looking for hands-on work in Chicago? Join our warehouse team. Consistent hours, supportive team, and room to grow. No experience? We’ll train you. Apply today!”

**Long:**
> “Join a growing logistics company in the greater Chicago area! We’re hiring Warehouse Associates for our day shift. Earn $17/hr+, enjoy a positive work culture, and get paid training from day one. Responsibilities include loading, order prep, and quality checks. If you’re reliable and ready to grow, we want to hear from you.”

---

## Future Development

- Tone variation by customer type (retail vs. tech vs. healthcare)
- AI-suggested A/B test variants
- Connection to Campaign Viewer feedback loop

---

> This generator ensures Hireway customers always launch with polished, high-performing job ads that reflect their brand and attract quality candidates.

File: `docs/recruiting/ad-copy-generator.md`
