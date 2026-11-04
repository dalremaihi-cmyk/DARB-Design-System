# DARB Student Components

## Responsible Member
Dana

## Overview

Research, design, and document reusable UI components for the student side of the DARB application. These components help students explore opportunities, manage their profiles, track applications, and receive personalized AI recommendations.

All components follow the DARB design system, using its approved color palette, IBM Plex Sans for English, Noto Sans Arabic for Arabic, and the approved outline icon library. Both English (LTR) and Arabic (RTL) layouts are supported.

## Tasks

### 1. Opportunity Components

- **Opportunity cards:** Display the opportunity title, organization, location, type, mode, and application deadline. Include actions such as saving an opportunity and viewing its details.
- **Card variations:** Design standard, saved, deadline-soon, and closed states.
- **Compact cards:** Create smaller versions for search results and lists, showing only the essential information.
- **Recommended opportunities:** Include an AI match percentage and a short explanation of why the opportunity is suitable for the student.
- **Opportunity categories:** Create reusable category chips with icons, names, and default and selected states. Categories may include internships, competitions, volunteering, events, and courses.

### 2. Student Components

- **Profile summary:** Display the student's photo or initials, name, university, major, and profile completion percentage. Include an edit action and complete and incomplete states.
- **Skills and interests:** Create reusable chips for skills and interests, including selected, removable, read-only, and empty states.
- **Saved opportunities:** Design simplified cards for saved opportunities, with active and expired states and a bookmark indicator.

### 3. Application Components

- **Status indicators:** Create status pills for Draft, Submitted, Under Review, Interview, Accepted, Not Selected, and Withdrawn. Each status uses an icon, text label, and appropriate color.
- **Application tracking:** Design a vertical stepper showing application stages, dates, and progress. Distinguish completed, current, and upcoming steps.
- **Deadline reminders:** Create reminder banners for normal, due-soon, closing-today, and closed opportunities.

### 4. AI Components

- **AI opportunity recommendations:** Design recommendation cards with an AI label, opportunity information, match reasons, and feedback actions such as Helpful and Not for me.
- **Suggested skills:** Create skill suggestion chips based on the student's courses and saved opportunities. Use a dashed outline to distinguish suggestions from confirmed skills, with Accept and Dismiss actions.

### 5. Design Requirements

- Use only the approved DARB color palette and typography styles.
- Use IBM Plex Sans for English and Noto Sans Arabic for Arabic.
- Use icons from the existing outline icon library at 16px, 20px, or 24px.
- Support both LTR and RTL layouts, mirroring directional icons in Arabic where required.
- Build components using Figma Auto Layout, reusable styles, and component properties.
- Maintain accessible touch areas of at least 44 × 44px for interactive elements.
- Pair status colors with icons and text so information is never communicated through color alone.
- Clearly label AI content and allow students to dismiss suggestions.

### 6. Documentation and Team Notes

Document each component's name, properties, variants, usage, and design rules. Keep the components consistent across Home, Explore, Profile, Saved, and Applications screens.

**Open items for the team:**
- The icon library does not currently include an AI or sparkle icon, so the `featured` star icon is used as a temporary replacement.
- The palette does not include an information status color, so Light Teal is used for in-progress states.
- The Secondary Text color `#5B6772` is a placeholder and needs confirmation because the original value is cropped in the brand board.

## Deliverables

- **Research and component requirements (Research-and-Requirements.pdf):** Defines the information, states, variations, and design requirements for each component.
- **Student component designs (Student UI components for DARB.pdf):** Shows visual examples of opportunity cards, profile components, skills, application tracking, deadline reminders, and AI recommendations.
- **Component documentation (Component-Documentation.pdf):** Lists component names, properties, variants, usage, and design rules.
- **Component variations:** Includes saved, expired, selected, deadline-soon, and application progress states.
- **Reusable Figma components:** Organize the designs into reusable components with properties and variants.
- **Final screenshots:** Capture the completed components and their variations for project documentation.

## Folder

`04-Student-Components/`

## Files
- `Research-and-Requirements.pdf`
- `Component-Documentation.pdf`
-  'DARB Student Components.md'


## Figma Link
[ DARB Student Components](https://www.figma.com/proto/RVLhXVfrgAPKWt2lkrfoAj/Untitled?node-id=3-31&p=f&t=2lapdV27pyfF4fmb-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A31
)
