# Student components

Reusable cards, chips, status indicators and AI suggestions for the student side of DARB. Every component is built from the DARB palette, IBM Plex Sans and Noto Sans Arabic, and the outline icon set, with English (LTR) and Arabic (RTL) versions.

## 1. Research and component requirements

What each component must show, and the states it needs. These come from the brand boards and the task list.

| Component | Information needed | Variants and states |
| --- | --- | --- |

### Inputs from the brand boards

- Colors only from the DARB palette. Status colors are always paired with an icon and text.
- Text uses the existing nine styles. Body text stays at 14px or larger. No uppercase or letter-spacing in Arabic.
- Outline icons at 16, 20 or 24px, at least 8px from text, with a 44 × 44px touch area when tappable.
- Arrows, chevrons, back and logout icons mirror in Arabic. Search, clock and check do not.

## 2. Opportunity components

### Opportunity card

### Compact card (lists and search results)

### Recommended opportunity

Adds a reason line. Use it in a horizontal carousel on Home.

### Opportunity category

## 3. Student components

### Profile summary

### Skills and interests

### Saved opportunity

## 4. Application components

### Status indicator

One pill with a status property. Each status has an icon and a text label, so color is never the only signal.

### Application tracking

### Deadline reminder

## 5. AI components

### AI opportunity recommendation

### Suggested skills

Suggested chips use a dashed outline so they never look like confirmed skills. Accept moves the chip to the skills list. Dismiss removes it and stops suggesting it.

## 6. Documentation

| Figma component | Properties | Usage |
| --- | --- | --- |

### Rules for every component

- Build with auto layout. Use color and text styles, never raw values or hand-set font sizes.
- Swap icon instances from the library. Do not redraw icons.
- Every EN component has an AR twin with the AR text style, mirrored layout and mirrored directional icons.
- Icon-only buttons need an accessible label. Tap targets are at least 44 × 44px.
- AI content is always labeled and always dismissible.

### Open items for the team

- The icon library has no AI or sparkle icon. This page uses `featured` (star) until one is added.
- The palette has no info status color. In-progress states use Light Teal.
- Confirm the Secondary Text hex. It is cropped in the board, so `#5B6772` is a placeholder here.