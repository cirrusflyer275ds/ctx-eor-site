# Platform Recommendations

This document outlines how Hireway recommends the best job advertisement platforms for each hiring campaign by leveraging structured data inputs and contextual logic.

---

## Goal

Deliver highly targeted, cost-effective platform recommendations based on the customer’s NAICS code, SOC (O\*NET) role, location, and budget. The goal is to connect with the *right workers* on the *right channels* with messaging that matches their motivations.

---

## Key Data Inputs

### 1. **NAICS Code (Industry Context)**

* Used to determine the sector and likely worker availability.
* Informs whether generalist or specialist platforms are most appropriate.

### 2. **O\*NET SOC Code (Job Function)**

* Maps to occupational families and job seeker behavior.
* Example: Production roles may perform better on Indeed, while technical roles may benefit from StackOverflow or GitHub Jobs.

### 3. **Geographic Data (Location Strategy)**

* ZIP code, city, or region determines:

  * Candidate density
  * Minimum wage thresholds
  * Commuting patterns

### 4. **Demographic Factors**

* Gender, age, income level, and internet usage by ZIP or metro area.
* Determines suitability of mobile-first platforms (e.g. Facebook vs. LinkedIn).

### 5. **Campaign Parameters**

* Budget (fixed or open-ended)
* Timeline to hire
* Ad type (evergreen vs. urgent burst)

---

## Logic for Recommendation

### Step 1: Industry-Specific Base Layer

* Match NAICS + SOC to standard recruiting platforms.
* Assign base score weights (e.g., 0.8 for Indeed in warehousing).

### Step 2: Geography and Demographics Adjustment

* Adjust scores based on:

  * Local workforce participation
  * Mobile vs. desktop usage
  * Education attainment levels

### Step 3: Final Weighting and Tiers

* Present top 3 platforms with reasoning:

  * Tier 1: Recommended primary spend
  * Tier 2: Optional channel expansion
  * Tier 3: Local or niche option

---

## Sample Output (for Warehouse Worker in Atlanta)

1. **Indeed** (Score: 9.2/10)

   * High concentration of entry-level job seekers in region
   * Proven response rates in logistics roles

2. **Facebook Ads** (Score: 8.7/10)

   * Dominant local use by working-age adults
   * Good match for visual messaging

3. **Craigslist ATL** (Score: 7.1/10)

   * Low cost per post
   * Historically active for similar roles

---

## Interface and Output Design

* Customers will see a visual recommendation card per platform
* Each card includes:

  * Platform name + logo
  * Key logic explanation ("Why here?")
  * CTA to allocate ad budget or edit parameters

---

## Future Enhancements

* Incorporate platform ROI tracking into loop
* Let customers vote up/down based on performance
* Real-time budget allocator based on early ad response

---

> This system turns data into decisions, helping customers spend smarter and hire faster.

