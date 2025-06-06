# Recreate the markdown file after code execution environment reset
refactored_md_content = '''---
title: "Trial Builder — Finalize & Share"
hide:
  - toc
---

# ✅ Finalize & Launch Your Trial Plan  
You're done! Here's a summary of your trial job configuration. You can save it, share it, or launch onboarding now.

---

## 📄 Trial Summary

**Company Name**: _{{ company_name }}_  
**Industry (NAICS)**: _{{ naics_description }}_  
**Role Selected**: _{{ job_title }}_  
**O*NET Mapping**: _{{ soc_code }} — {{ soc_title }}_  
**Tasks Selected**: {{ task_count }}  
**Skills Chosen**: {{ skill_count }}  
**Trial Length**: {{ trial_length }} Days  
**Check-ins**: {{ check_in_schedule }}  
**Custom Requirements**: {{ special_requirements }}

---

## ✏️ Name Your Trial

Give your trial a clear internal name:  
> Example: **Day Shift Coordinator (July Start)**

`[ ____________________________ ]`

---

## 👥 Share with Your Team

Who should receive updates, reports, and onboarding alerts?

- [ ] Email a copy
- [ ] Copy shareable link
- [ ] Print trial summary

_Add recipient emails:_  
`[ {{ primary_contact_email }}, {{ backup_contact_email }} ]`

---

## 💾 Save or Launch

Once saved, your trial template will be:
- Stored in your dashboard  
- Available to reuse or clone  
- Linked to onboarding and payroll setup

> **Next**, we'll walk you through candidate onboarding. Hireway becomes the legal employer — you manage the work, we handle compliance.

✅ It's fast.  
✅ It's safe.  
✅ It's smart trial hiring.

---

## ⚙️ Advanced Evaluation Checkpoint Customization (Optional)

If you'd like to customize how and when feedback is collected during the trial:

### 📅 When to Evaluate?
- [ ] After 3 days (Early signal)
- [ ] After 1 week
- [x] After 2 weeks
- [x] At 30 days (Full cycle)
- [ ] End of trial (only)

### 👤 Who Should Provide Feedback?
- [x] Direct Supervisor
- [ ] Peer or Co-worker
- [ ] Team Lead or Floor Manager
- [ ] Site Contact or Field Manager

### 📝 What Do You Want Scored?
- [x] Work quality
- [x] Task completion speed
- [x] Attendance and punctuality
- [x] Attitude / coachability
- [ ] Communication skills
- [ ] Safety or rule compliance

### 🔍 Add Optional Prompts?
- [ ] Include open-ended feedback field
- [ ] Include 1–5 rating scale
- [ ] Flag “go / no-go” recommendation box

---

[← Back to Check-ins](trial-builder-step9.md)  
[Save & Start Onboarding](#)
'''

# Save to file
file_path = "/mnt/data/trial-finalize-and-share-template.md"
with open(file_path, "w") as f:
    f.write(refactored_md_content)

file_path
