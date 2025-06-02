---
title: Step 8 – Background Check & Screening
hide:
  - toc
---

# 🔍 Step 8: Background Check & Screening

When required by the employer, we handle background checks and drug screenings seamlessly — with full transparency and candidate control.

---

## What Happens in This Step

1. **Disclosure & Authorization**  
   Candidates are shown a digital version of the Fair Credit Reporting Act (FCRA) disclosure and authorization form.

2. **Background Screening via Checkr**  
   Upon acknowledgment, we trigger a background check using our Checkr integration.

3. **Optional Drug Screening**  
   If required by the employer, the candidate selects a testing location and time.

4. **Appointment Confirmation & Reminder Flow**  
   Candidates receive SMS/email reminders. Missed appointments trigger a support escalation.

---

## Key Features

✅ Mobile-friendly Checkr authorization  
✅ Candidate picks time & location for testing  
✅ Confirmation reminders with acknowledgment  
✅ Escalation to Hireway rep if issues arise  
✅ All results securely stored & shared with authorized users only

---

## Why It Matters

This step ensures the employer meets all pre-hire compliance requirements — without chasing down paperwork or managing vendors.

---

## Built-In Logic

- If no background check is required, this step is skipped.
- If drug screening is required:
  - Candidate picks a nearby clinic via Checkr API
  - We monitor appointment status
- Candidate acknowledgment is logged and included in final PDF

---

[Next: Health Insurance & Benefits →](onboarding-step-9-benefits.md)
