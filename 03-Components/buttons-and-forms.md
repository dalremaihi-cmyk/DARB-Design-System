# DARB Buttons and Forms

## Responsible Member
Haya

## Overview
Research and design reusable buttons and form components
for the DARB application.

## Tasks

### Buttons
- Identify the button types needed in DARB.
- Design primary and secondary buttons.
- Design different button states.
- Ensure consistency across the application.

# 1. Button Types Needed in DARB

| # | Type | Purpose | DARB Example |
|---|------|---------|--------------|
| 1 | Primary | The one main action on a screen | "Apply Now", "Publish", "Submit" |
| 2 | Secondary | Supporting action | "Save Draft", "Cancel", "View Details" |
| 3 | Tertiary / Text | Low-emphasis inline action | "Edit", "Show more", "Read eligibility" |
| 4 | Ghost | On colored/dark surfaces | "Log out", "Dismiss" |
| 5 | Destructive | Irreversible action | "Withdraw Application", "Delete", "Reject" |
| 6 | Icon | Compact utility | 🔔 notifications · 🔍 filter · 💬 message · ✕ close |
| 7 | Split / Dropdown | Action with options | "Message ▾", "Change Status ▾" |
| 8 | Link | Navigation styled as text | "Read eligibility criteria" |
| 9 | Toggle / Segmented | Switch views | "All \| Eligible \| Applied" |
| 10 | FAB | Mobile primary shortcut | "＋ Post" (staff), "＋ Quick Apply" (student) |
| 11 | File / Upload | Trigger file picker | "Upload CV", "Add Certificate" |

# Summary Count

| Metric | Value |
|--------|-------|
| Button types | 11 |
| Distinct usages | ~50+ across 9 screen contexts |
| Most frequent | Primary (~10 screens), Secondary (~9 screens) |
| Reserved for safety | Destructive (4 flows, always confirmed) |

# Where Primary Appears

| Screen | Primary Button |
|--------|----------------|
| Opportunity feed | "Apply Now" (on card) |
| Apply form | "Submit Application" |
| Application detail | "Submit Application" (draft) |
| Post opportunity (staff) | "Publish Opportunity" |
| Review submissions (staff) | "Approve" |
| Messaging (staff) | "Send Message" |
| Confirm dialog | "Confirm" |
| Request opportunity (F12) | "Submit Request" |


# Where Secondary Appears

| Screen | Secondary Button |
|--------|------------------|
| Any form | "Cancel" |
| Apply form | "Save Draft" |
| Opportunity card | "View Details" |
| Profile | "Edit Profile" |
| Notifications | "Mark all as read" |
| Post opportunity | "Save as Draft", "Preview" |
| Review | "Request More Info" |

# Primary Button — State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#173B57` | `#FFFFFF` | none | — | pointer |
| Hover | `#1F4E70` | `#FFFFFF` | none | — | pointer |
| Active (pressed) | `#0F2C42` + scale 0.98 | `#FFFFFF` | none | — | pointer |
| Focus (keyboard) | `#173B57` | `#FFFFFF` | none | `3px #8FB4CC`, offset 2px | pointer |
| Disabled | `#EDF1F4` | `#98A4B0` | none | — | not-allowed |
| Loading | `#173B57` (90% opacity) | `#FFFFFF` + spinner | none | — | wait |
| Success (transient) | `#247A4B` + ✓ | `#FFFFFF` | none | — | pointer |

#  Secondary Button — State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#173B57` | `1.5px #173B57` | — | pointer |
| Hover | `#E3EBF1` | `#173B57` | `1.5px #173B57` | — | pointer |
| Active (pressed) | `#D6E1EA` + scale 0.98 | `#0F2C42` | `1.5px #0F2C42` | — | pointer |
| Focus (keyboard) | `#FFFFFF` | `#173B57` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | pointer |
| Disabled | `#F6F8FA` | `#98A4B0` | `1.5px #DCE3EA` | — | not-allowed |
| Loading | `#FFFFFF` | `#173B57` + spinner | `1.5px #173B57` | — | wait |
### Form Components
- Design text input fields.
- Design search bars.
- Design dropdown menus.
- Design checkboxes and radio buttons.
- Design date selection components.
- Consider validation and error states.
# Shared Form Foundations

| Token | Value |
|-------|-------|
| field.height.md | 40px |
| field.height.lg | 48px |
| field.radius | 8px |
| field.padding-x | 12px |
| label.gap | 6px |
| helper.gap | 6px |
| field.gap | 20px |
| section.gap | 32px |

# Text Input Fields — State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#202B35` | `1.5px #DCE3EA` | — | text |
| Hover | `#FFFFFF` | `#202B35` | `1.5px #B8C4D0` | — | text |
| Focus | `#FFFFFF` | `#202B35` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | text |
| Filled | `#FFFFFF` | `#202B35` | `1.5px #DCE3EA` | — | text |
| Success (async) | `#FFFFFF` | `#202B35` | `1.5px #176B6B` | — | text |
| Disabled | `#F6F8FA` | `#98A4B0` | `1.5px #EDF1F4` | — | not-allowed |
| Read-only | `#F6F8FA` | `#5B6775` | `1.5px dashed #DCE3EA` | — | default |
| Error | `#FCEDEC` | `#202B35` | `1.5px #B42318` | — | text |
| Loading | `#FFFFFF` | `#202B35` | `1.5px #DCE3EA` | — | wait |

# Trigger State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#5B6775` | `1.5px #DCE3EA` | — | pointer |
| Hover | `#FFFFFF` | `#5B6775` | `1.5px #B8C4D0` | — | pointer |
| Focus/Open | `#FFFFFF` | `#202B35` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | pointer |
| Selected | `#FFFFFF` | `#202B35` | `1.5px #DCE3EA` | — | pointer |
| Disabled | `#F6F8FA` | `#98A4B0` | `1.5px #EDF1F4` | — | not-allowed |
| Error | `#FCEDEC` | `#202B35` | `1.5px #B42318` | — | pointer |

# Menu Item State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#202B35` | none | — | pointer |
| Hover | `#D9F0ED` | `#173B57` | none | — | pointer |
| Selected | `#D9F0ED` | `#173B57` + ✓ `#176B6B` | none | — | pointer |
| Disabled | `#FFFFFF` | `#98A4B0` | none | — | not-allowed |
| Focus (keyboard) | `#D9F0ED` | `#173B57` | none | `3px #8FB4CC` inset | pointer |

# Checkboxes State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#202B35` | `1.5px #B8C4D0` | — | pointer |
| Hover | `#FFFFFF` | `#202B35` | `1.5px #173B57` | — | pointer |
| Focus | `#FFFFFF` | `#202B35` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | pointer |
| Checked (consent) | `#173B57` | `#FFFFFF` | none | — | pointer |
| Checked (filter) | `#176B6B` | `#FFFFFF` | none | — | pointer |
| Indeterminate | `#173B57` | `#FFFFFF` | none | — | pointer |
| Disabled | `#EDF1F4` | `#98A4B0` | `1.5px #DCE3EA` | — | not-allowed |
| Error (group) | `#FFFFFF` | `#202B35` | `1.5px #B42318` | — | pointer |

# Radio Buttons — State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#202B35` | `1.5px #B8C4D0` | — | pointer |
| Hover | `#FFFFFF` | `#202B35` | `1.5px #173B57` | — | pointer |
| Focus | `#FFFFFF` | `#202B35` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | pointer |
| Selected | `#FFFFFF` | `#202B35` | `1.5px #173B57` + inner dot `#176B6B` | — | pointer |
| Disabled | `#EDF1F4` | `#98A4B0` | `1.5px #DCE3EA` | — | not-allowed |
| Error (group) | `#FFFFFF` | `#202B35` | `1.5px #B42318` | — | pointer |

# Date Selection —  Trigger State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#5B6775` | `1.5px #DCE3EA` | — | pointer |
| Hover | `#FFFFFF` | `#5B6775` | `1.5px #B8C4D0` | — | pointer |
| Focus/Open | `#FFFFFF` | `#202B35` | `1.5px #173B57` | `3px #8FB4CC`, offset 2px | pointer |
| Filled | `#FFFFFF` | `#202B35` | `1.5px #DCE3EA` | — | pointer |
| Disabled | `#F6F8FA` | `#98A4B0` | `1.5px #EDF1F4` | — | not-allowed |
| Error | `#FCEDEC` | `#202B35` | `1.5px #B42318` | — | pointer |

# Date Selection — Calendar Day Cell State Table

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Default | `#FFFFFF` | `#202B35` | none | — | pointer |
| Hover | `#D9F0ED` | `#173B57` | none | — | pointer |
| Today | `#FFFFFF` | `#202B35` | `1.5px #176B6B` | — | pointer |
| Selected | `#173B57` | `#FFFFFF` | none | — | pointer |
| In range | `#D9F0ED` | `#173B57` | none | — | pointer |
| Range endpoint | `#173B57` | `#FFFFFF` | none | — | pointer |
| Disabled (past) | `#FFFFFF` | `#98A4B0` | none | — | not-allowed |
| Outside month | `#FFFFFF` | `#B8C4D0` | none | — | pointer |
| Focus (keyboard) | `#FFFFFF` | `#202B35` | none | `3px #8FB4CC`, offset 2px | pointer |

# Validation & Error States —  Error State Table (applies to all fields)

| State | Background | Text | Border | Outline | Cursor |
|-------|------------|------|--------|---------|--------|
| Error (input) | `#FCEDEC` | `#202B35` | `1.5px #B42318` | — | text |
| Error (helper) | — | `#B42318` | none | — | default |
| Success (input) | `#FFFFFF` | `#202B35` | `1.5px #176B6B` | — | text |
| Success (helper) | — | `#176B6B` | none | — | default |

# DARB-Specific Rules

| Field | Rule | Message |
|-------|------|---------|
| University email | Domain check | "Use your university email address." |
| CV | PDF, ≤ 10 MB | "CV must be a PDF under 10 MB." |
| Certificates | PDF/JPG/PNG, ≤ 5 MB × 5 | "Upload up to 5 files (PDF/JPG/PNG, max 5 MB each)." |
| Deadline | Future | "Deadline must be in the future." |
| Date range | To ≥ From | "End date must be after start date." |
| GPA | 0–4.0 | "GPA must be between 0 and 4.0." |
| Year | 1–6 | "Select a valid year of study." |
| Title | 5–120 chars | "Title must be 5–120 characters." |
| Eligibility | ≥1 major + ≥1 year | "Select at least one major and one year." |
| Duplicate apply | Not already applied | "You have already applied to this opportunity." |

## Deliverables
- Research and component requirements.
- Reusable Figma components.
- Component variations and states.
- Component documentation.
- Screenshots of the final work.

## Folder
03-Components/

## Figma Link
To be added.
