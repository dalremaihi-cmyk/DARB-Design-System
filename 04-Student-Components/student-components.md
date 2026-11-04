# DARB Student Components

## Responsible Member
Dana

## Overview
Research, design, and document reusable UI components for the student side of the DARB application. The purpose of this work is to create a consistent and user-friendly interface that helps students explore opportunities, manage their profiles, track applications, and receive personalized recommendations.

The components are designed to be reusable across different screens of the application, reducing repeated design work and maintaining a consistent appearance. The designs support both English (Left-to-Right) and Arabic (Right-to-Left) layouts and follow the DARB design system, including its approved color palette, typography, and icon style.

## Tasks

### Opportunity Components

- [x] **Identify the information needed in opportunity cards.**
  - Determine the essential information students need when browsing opportunities, including opportunity type, title, organization name, location, opportunity mode, and application deadline.
  - Identify the main actions required, such as saving an opportunity and viewing its details.
  - Identify optional information, including required skills and AI match scores.

- [x] **Design opportunity cards with different states.**
  - Create a standard card displaying the opportunity information in an organized layout.
  - Design a saved state that visually indicates when a student has bookmarked an opportunity.
  - Create a deadline-soon state to highlight opportunities approaching their application deadline.
  - Design a closed state for opportunities that are no longer accepting applications.
  - Include English and Arabic versions.

- [x] **Design recommended opportunity cards with match scores and reasons.**
  - Create a card that highlights opportunities recommended to students.
  - Include a match percentage to show how closely an opportunity matches the student's skills and interests.
  - Add a short explanation describing why the opportunity is recommended.
  - Design the card for use in the Home screen recommendation carousel.

- [x] **Design opportunity category components.**
  - Create category chips with an icon and category name.
  - Include categories such as internships, competitions, volunteering, events, courses, and university opportunities.
  - Design default and selected states to help students identify active filters.
  - Include optional counts showing the number of opportunities in each category.

- [x] **Create compact opportunity card variations.**
  - Design smaller card layouts for lists and search results.
  - Display the most important information, including the opportunity title, organization, location, and deadline.
  - Keep the layout simple while maintaining consistency with the standard opportunity card.

### Student Components

- [x] **Design student profile components with completion indicators.**
  - Create a profile summary displaying the student's photo or initials, name, university, and major.
  - Include a profile completion percentage to show how much of the student's profile has been completed.
  - Add an edit profile action to allow students to update their information.
  - Design default, incomplete, and complete profile states.

- [x] **Design skills and interests components.**
  - Create reusable skill chips to display the student's skills and interests.
  - Include different states such as read-only, selected, removable, and add skill.
  - Design an empty state for students who have not added any skills.
  - Include a suggested state for skills recommended by DARB AI.

- [x] **Design saved opportunity components with active and expired states.**
  - Create a simplified card for opportunities saved by students.
  - Include important opportunity information and a bookmark indicator.
  - Design an active state for opportunities that are still available.
  - Design an expired state for opportunities that have passed their deadline or are no longer available.

### Application Components

- [x] **Design application status indicators.**
  - Create reusable status indicators that communicate the current stage of an application.
  - Include statuses such as Draft, Submitted, Under Review, Interview, Accepted, Not Selected, and Withdrawn.
  - Use different status colors, icons, and text labels to make each status easy to recognize.
  - Ensure that status information is not communicated through color alone.

- [x] **Design application tracking components.**
  - Create a vertical stepper that displays the progress of a student's application.
  - Include the application stages, relevant dates, and current status.
  - Distinguish between completed, current, and upcoming steps.
  - Help students understand their application progress and identify the next stage.

- [x] **Design deadline reminder components with different urgency states.**
  - Create reminder banners that display the application deadline and remaining time.
  - Design a normal state for deadlines that are more than seven days away.
  - Create a due-soon state to highlight opportunities approaching their deadlines.
  - Design a closing-today state that reminds students to submit their applications before the deadline.
  - Include a closed state explaining that applications are no longer available.

### AI Components

- [x] **Identify suitable components for AI recommendations.**
  - Identify reusable components that can display personalized opportunity recommendations.
  - Determine how AI suggestions can be presented without making the interface confusing.
  - Identify the information required to explain recommendations, including matching skills and student interests.
  - Consider feedback actions that allow students to respond to recommendations.

- [x] **Design AI opportunity recommendation components.**
  - Create recommendation cards with an AI label to distinguish them from regular opportunities.
  - Include the opportunity title, organization, location, and recommendation reason.
  - Display why an opportunity matches the student's skills or interests.
  - Add feedback actions such as Helpful and Not for me.
  - Allow students to dismiss recommendations they are not interested in.

- [x] **Design suggested skills components with accept and dismiss actions.**
  - Create skill suggestion chips based on the student's courses and saved opportunities.
  - Display suggested skills such as Data Analysis, SQL, and Public Speaking.
  - Include Accept and Dismiss actions so students can manage suggestions.
  - Use a dashed outline to distinguish suggested skills from skills already added to the profile.
  - Ensure accepted skills can be added to the student's profile and dismissed suggestions can be removed.

### Design Requirements

- [x] **Apply the DARB color palette and typography.**
  - Use the approved DARB color tokens to maintain consistency across components.
  - Apply IBM Plex Sans for English text and Noto Sans Arabic for Arabic text.
  - Follow the established typography hierarchy for headings, body text, labels, and captions.

- [x] **Use the approved outline icon style.**
  - Use icons from the DARB icon library instead of creating inconsistent icon designs.
  - Follow the defined icon sizes of 16px, 20px, and 24px.
  - Maintain consistent spacing between icons and text.

- [x] **Prepare English and Arabic component layouts.**
  - Create English versions using left-to-right layouts.
  - Create Arabic versions using right-to-left layouts.
  - Ensure text alignment and component positioning are appropriate for each language.

- [x] **Follow right-to-left layout rules for Arabic.**
  - Mirror directional elements such as arrows and chevrons.
  - Maintain the correct Arabic text alignment.
  - Keep icons such as search, clock, and check in their original orientation.

- [x] **Define component variants, states, and usage guidelines.**
  - Document the available properties and variations for each reusable component.
  - Define where each component should be used, such as Home, Explore, Profile, Saved, and Applications.
  - Establish consistent design rules for spacing, typography, colors, icons, and accessibility.
  - Ensure interactive elements have a minimum touch area of 44 × 44px.

## Deliverables

- [x] **Research and component requirements (Research-and-Requirements.pdf)**
  - Documents the required information, states, and variations for each student component.
  - Includes the main design requirements and brand guidelines.

- [x] **Student component designs and examples (Student UI components for DARB.pdf)**
  - Contains visual examples of opportunity cards, profile components, skills, application tracking, deadline reminders, and AI recommendations.
  - Shows different component states and English and Arabic layouts.

- [x] **Component documentation (Component-Documentation.pdf)**
  - Lists the component names, available variants, and where each component will be used in the application.
  - Includes general rules for maintaining consistency across the designs.

- [x] **Component variants and states documented.**
  - Documents variations such as saved, expired, selected, deadline soon, accepted, dismissed, and application progress states.

- [ ] **Reusable Figma components.**
  - Organize the final designs as reusable Figma components with clearly defined properties and variants.

- [ ] **Screenshots of the final Figma work.**
  - Capture screenshots of the completed Figma components and their variations for the final project documentation.

## Folder
04-Student-Components/

## Files
- Research-and-Requirements.pdf
- Component-Documentation.pdf
- Student UI components for DARB.pdf

## Figma Link
https://www.figma.com/design/RVLhXVfrgAPKWt2lkrfoAj/Untitled?node-id=0-1&t=e9iPnw5EXhf23g4D-1
