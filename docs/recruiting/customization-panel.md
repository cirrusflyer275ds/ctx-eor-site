# Customization Panel

This module outlines how CTX-EOR customers can fine-tune their recruiting campaigns through a guided customization interface.

---

## Purpose

- Allow customers to adjust ad copy, targeting, and evaluation logic
- Support both default and advanced settings
- Provide transparency into what’s being customized and why

---

## Key Customization Areas

1. **Ad Voice & Tone**
   - Formal, casual, benefits-forward, mission-driven, etc.
   - Informed by industry/SOC norms + customer preferences

2. **Candidate Filters**
   - Geography radius
   - Prior experience required
   - Education minimum
   - Soft skill emphasis

3. **Interview Preferences**
   - Pre-recorded vs live Zoom interview
   - Question topics and traits to emphasize
   - Pass/fail criteria (if any)

4. **Platform Biasing**
   - Preference for specific job boards
   - Budget weighting across platforms

5. **Scoring Adjustments**
   - Customer can apply “boost” to certain traits or answers
   - Example: give higher weight to reliability or availability

---

## Interface Layout (Placeholder)

- Step-by-step panel (wizard-style)
- Smart defaults based on NAICS, SOC, and prior campaigns
- Real-time preview of campaign summary
- Optional “Expert Assist” mode for CTX-EOR staff to review settings

---

## Underlying Logic

Customization preferences will alter:
- LLM prompt templates
- Job board targeting config
- Screening algorithm weighting

---

> This is a scaffold for customer-facing customization. The backend config mapping will be defined separately.


