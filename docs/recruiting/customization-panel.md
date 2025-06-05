# Customization Panel

This module outlines how Hireway customers can fine-tune their recruiting campaigns through a guided customization interface.

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

# Customization Panel

The Customization Panel allows customers to fine-tune how their job ad campaign is built and deployed—without needing to understand recruiting technology or write ad copy manually.

---

## Overview

This panel is designed for customers who want to:
- Modify the tone or style of ad copy
- Choose or exclude certain advertising platforms
- Adjust spending allocations across platforms
- Provide input on targeting priorities (e.g., speed, diversity, experience)

---

## Key Features

### 1. Voice & Tone Adjustments
Customers choose how they want to sound to potential applicants:
- ✅ Culture-forward
- ✅ Professional & polished
- ✅ Blue-collar relatable
- ✅ Urgency-driven
- ✅ Custom upload / use previous style

*Behind the scenes, a prompt is adjusted for the ad-copy generator.*

---

### 2. Budget Tweaking

Customers see the default recommendation from the Placement Engine, but can override:
- Total budget
- Budget by platform (e.g., 40% Facebook, 30% Craigslist)
- Budget duration (weekly or monthly)

---

### 3. Platform Preferences

Let customers:
- Exclude platforms they don’t like
- Prioritize niche boards (e.g., Stack Overflow, Behance, HealthJobs)
- Set preferred frequency of refresh / repost

---

### 4. Targeting Goals

Sliders and toggle options allow for:
- ⚖️ Speed vs. cost balance
- 🎯 Narrow vs. broad targeting
- 👥 Diversity & inclusion goals (optional)

---

## User Interface Concept

The panel will use:
- Sliders for tones and targeting weights
- Editable textboxes for budget
- Toggle chips for platform inclusion/exclusion
- LLM-generated explanations of "what this setting does"

---

## Why This Matters

- Increases customer confidence
- Reduces friction around budget decisions
- Aligns recruiting with company values and brand voice

---

## Integration with Ad Generator

The output from this panel feeds directly into the:
- Ad-Copy Generator prompt structure
- Placement Engine targeting strategy
- Campaign preview shown to customer

---

> This panel turns complex campaign logic into simple, understandable choices. Customers stay in control without needing to learn recruiting software.

---

File location: `docs/recruiting/customization-panel.md`

