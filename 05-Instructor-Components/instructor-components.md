# DARB Instructor Components

## Responsible Member
Jawaher Jabr Al-Aji

## Overview
This section defines and documents the reusable user interface (UI) components designed specifically for the instructor and administrator side of the DARB platform. These components empower faculty members, opportunity creators, and department administrators to publish opportunities, review incoming student applications, manage participant pipelines, and track academic engagement.

All components adhere strictly to the DARB design system foundation: using the approved brand color palette (01-Branding), IBM Plex Sans for English (LTR), Noto Sans Arabic for Arabic (RTL), and the 36-icon outline library. High-density layouts, clear data tables, and batch-action patterns ensure efficiency during administrative workflows.

## Tasks

### Opportunity Management
**Opportunity Creation Form Components:**

Design multi-step form elements: basic details (title, department, category), eligibility parameters (GPA threshold, required majors, year levels), capacity limits, and deadline selectors.

Include interactive state inputs: empty, focused, filled, error validation, and multi-select dropdowns for target majors.

**Opportunity Management Cards & Dashboard Rows:**

Create list rows and card views showing opportunity status, active applicant counts, views, and publish dates.

Include quick action buttons: View Applicants, Edit, Duplicate, Pause Applications, and Archive.

**Opportunity Editing Components:**

Design inline quick-edit modals and full edit page forms with state indicators: Published (Live), Draft, Closed/Expired, and Archived.

### Applicant Management
**Applicant Profile Cards & Drawer Views:**

Design compact and detailed applicant cards displaying student photo/initials, name, major, academic year, GPA, attached resume link, and submission timestamp.

**Application Status Indicators & Pills:**

Create standardized status pills: Draft, Submitted, Under Review, Shortlisted, Interview Scheduled, Accepted, Rejected, and Withdrawn. Each pill pairs a distinct background color, outline icon, and text label.

**Application Review Components:**

Design split-view review screens: student submission preview on the left/right, and evaluation/feedback forms, scorecards, and action buttons (Approve, Reject, Request Info) on the side panel.

### Student Management
**Student Search Components:**

Create search bars with autocomplete major tags, keyword highlights, and recent search history dropdowns.

**Student Filtering Components:**

Design filter panels and popovers supporting filter criteria: Major/Department, Academic Year (Freshman–Senior), Skills, Minimum GPA, and Application Status. Includes filter active/cleared states and badge counters.

**Student Information & Talent Directory Components:**

Design table views and roster cards displaying candidate summary cards for candidate discovery across the department.

## Component Hierarchy & Status Indicators

### Application Status Palette & Icons

| Status Pill | Token / HEX | Icon | Usage / Context |
| :--- | :--- | :--- | :--- |
| **Submitted / New** | `brand.secondary` (`#176B6B`) | `Icon/Actions/document` | Newly received applications pending evaluation |
| **Under Review** | `status.warning` (`#9A6500`) | `Icon/Status/info` | Currently being evaluated by faculty/committee |
| **Shortlisted / Interview** | `brand.primary` (`#202B35`) | `Icon/Opportunities/team` | Candidates selected for secondary screening |
| **Accepted / Approved** | `status.success` (`#247A4B`) | `Icon/Status/success` | Student officially accepted into the opportunity |
| **Rejected / Declined** | `status.error` (`#B42318`) | `Icon/Status/error` | Application declined |
| **Closed / Archived** | `neutral.text-secondary` (`#5B6775`) | `Icon/Actions/close` | Opportunity no longer accepting submissions |

### Design Requirements & RTL Rules
Color & Typography Integrity: Use only approved DARB color tokens and text hierarchy styles (EN/Heading/H1, AR/Heading/H1, type.body.default, etc.).

Dual-Language Alignment: Standardize on IBM Plex Sans for English (LTR) and Noto Sans Arabic for Arabic (RTL). Arabic layouts mirror navigation and directional chevrons while maintaining right-aligned text.

Interactive Touch Targets: Ensure all buttons, status drop-downs, and table action icons maintain an accessible minimum hit area of 44 × 44px.

Data Accessibility: Never convey status by color alone; pair every status pill with an explicit text label and icon component.

### Documentation & Open Items
**Documentation:**
Full component properties, Auto Layout configurations, component variants, and variant matrices are logged in Component-Documentation.pdf.

**Open Items for Team Review:**

Need team decision on adding a dedicated "Export to CSV/Excel" icon variant for applicant roster management.

Review whether Shortlisted status needs a unique brand color token to stand out from default primary dark navy buttons.


## Deliverables
Research & Requirements (Research-and-Requirements.pdf): Defines instructor requirements, administrative workflows, and component specifications.

Component Documentation (Component-Documentation.pdf): Details component names, variant parameters, Auto Layout specs, and usage guidelines.

DARB Instructor Components Summary (DARB Instructor Components.md): Complete Markdown reference for the repository.

Reusable Figma Components: Clean Figma library featuring Auto Layout components with properties, interactive states, and LTR/RTL variants.

Final Screenshots: High-resolution screenshots showcasing component boards, variant sets, and screen implementations.

## Folder
* 05-Instructor-Components/
  * Research-and-Requirements.pdf
  * Component-Documentation.pdf
  * DARB Instructor Components.md
  * Screenshots/
    * instructor-opportunity-components.png
    * applicant-management-components.png
    * student-filtering-components.png

## Figma Link
To be added.
