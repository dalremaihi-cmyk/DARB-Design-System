# DARB Typography & Icon Guidelines

## Responsible Member
Lolwa Al-Hemaidi

## 1. Overview

This section defines how text and icons look across the DARB application. It builds on the **Branding & Colors** foundation (01-Branding) — all text and icon colors use the approved DARB color tokens.

DARB is bilingual, so every text style has an **English (EN)** and an **Arabic (AR)** version that work together in left-to-right and right-to-left layouts.

## 2. Font Research

### English font options

| Font | Strengths | Weaknesses |
|---|---|---|
| **IBM Plex Sans** | Professional, very readable on screens, 4 clear weights, has a matching Arabic family | Slightly wider than Inter |
| Inter | Very clean UI font, excellent at small sizes | No Arabic version — pairing is less consistent |
| Roboto | Familiar Android default | Feels generic, weaker brand personality |

### Arabic font options

| Font | Strengths | Weaknesses |
|---|---|---|
| IBM Plex Sans Arabic | Designed to match IBM Plex Sans | Not available in Figma's built-in fonts — every team member would need to install it |
| **Noto Sans Arabic** | Clean and modern, built into Figma, wide weight range, very readable | Slightly more neutral in character |
| Cairo / Tajawal | Friendly and popular | Less balanced next to IBM Plex Sans |

Comparison criteria: readability at 12–14px, number of weights, balance between Arabic and English, free license (all options are open-source Google Fonts), and availability in Figma for the whole team.

## 3. Selected Fonts

| Language | Font | Weights used | Direction |
|---|---|---|---|
| English | **IBM Plex Sans** | Regular 400, Medium 500, SemiBold 600, Bold 700 | LTR |
| Arabic | **Noto Sans Arabic** | Regular 400, Medium 500, SemiBold 600, Bold 700 | RTL |

**Why:** IBM Plex Sans is professional and trustworthy while staying friendly, which matches the DARB brand personality. Noto Sans Arabic pairs well with it and is available to everyone in Figma without installing anything. Both fonts are free from Google Fonts.

## 4. Typography Hierarchy (Type Scale)

Sizes are in px, written as **size / line height**.

| Token | Figma style | English | Arabic | Use |
|---|---|---|---|---|
| `type.display` | Display | 32 / 40 · Bold | 32 / 44 · Bold | Hero titles, onboarding |
| `type.heading.h1` | Heading/H1 | 24 / 32 · SemiBold | 24 / 36 · SemiBold | Screen titles |
| `type.heading.h2` | Heading/H2 | 20 / 28 · SemiBold | 20 / 32 · SemiBold | Section titles |
| `type.heading.h3` | Heading/H3 | 18 / 24 · SemiBold | 18 / 28 · SemiBold | Card and dialog titles |
| `type.body.large` | Body/Large | 16 / 24 · Regular | 16 / 28 · Regular | Long reading text, descriptions |
| `type.body.default` | Body/Default | 14 / 20 · Regular | 14 / 24 · Regular | Default UI text, input text |
| `type.label` | Label | 14 / 20 · Medium | 14 / 24 · Medium | Buttons, form labels, tabs |
| `type.caption` | Caption | 12 / 16 · Regular | 12 / 20 · Regular | Metadata, helper and error text |
| `type.overline` | Overline | 11 / 16 · SemiBold · UPPERCASE · +8% spacing | 12 / 20 · SemiBold | Category tags, small section labels |

In Figma, styles are named `EN/<style>` and `AR/<style>` (for example `EN/Heading/H1` and `AR/Heading/H1`).

## 5. Text Colors

Text uses only colors from the DARB palette:

| Use | Token | HEX |
|---|---|---|
| Headings, body, labels | `neutral.text-primary` | #202B35 |
| Metadata, helper text | `neutral.text-secondary` | #5B6775 |
| Links, text buttons | `brand.secondary` | #176B6B |
| Text on Primary Blue | `neutral.white` | #FFFFFF |
| Error / success / warning messages | `status.error` / `status.success` / `status.warning` | #B42318 / #247A4B / #9A6500 |

## 6. Typography Guidelines

- Use text styles only — never set font sizes by hand.
- Minimum text size is 12px; keep body text at 14px or larger.
- Use sentence case for headings and buttons.
- Limit each screen to about three text sizes.
- Never show status with color alone — add text or an icon.

### Arabic & RTL rules
- Every EN style has a matching AR style — always use the pair.
- Align Arabic text to the right and mirror the layout.
- No letter-spacing and no uppercase in Arabic.
- Arabic line heights are 4px taller to leave room for diacritics.
- Use one number style per screen (Arabic-Indic ٠١٢ or Western 012).

## 7. Icons

### Icon library research

| Option | Notes |
|---|---|
| Material Symbols | Huge set, but looks very "Google/Android" |
| Phosphor / Lucide | Clean outline styles, close to the DARB brand board |
| **Custom DARB set (selected)** | 36 outline icons drawn in Figma in the Lucide/Phosphor style, so they match the brand exactly and have no licensing issues |

### Icon style
- Outline icons on a **24 × 24px** grid
- **1.75px** stroke with rounded ends and corners
- No filled icons mixed in

### Icon collection (36 icons)

| Group | Icons |
|---|---|
| Navigation | home, explore, search, saved, profile, menu, notifications |
| Opportunities | internship, competition, volunteering, event, university, course, team |
| Actions | filter, add, edit, upload, document, share, arrow-forward, chevron-back, chevron-forward, check, close, logout |
| Status | success, warning, error, info |
| Details | location, deadline, email, password, show, featured |

Each icon is a Figma component named `Icon/<Group>/<name>` (for example `Icon/Opportunities/internship`).

### Icon sizes

| Token | Size | Use |
|---|---|---|
| `icon.size.sm` | 16px | Next to captions and inside tags |
| `icon.size.md` | 20px | Inside buttons and text inputs |
| `icon.size.lg` | 24px | Navigation bar, headers, list items |

Tappable icons need a touch area of at least **44 × 44px**.

### Icon colors

| Use | Token |
|---|---|
| Default | `neutral.text-primary` |
| Muted / inactive tab | `neutral.text-secondary` |
| Active / selected | `brand.secondary` |
| On Primary Blue | `neutral.white` |
| Status icons | matching `status.*` color |

### Icon guidelines
- Use the icon components — don't stretch, rotate or redraw icons.
- Always pair status icons with a text message.
- Icon-only buttons need an accessible label.
- Keep at least 8px between an icon and its text.
- **RTL:** flip directional icons in Arabic (arrows, chevrons, back, logout). Don't flip icons like search, clock, or check.

## 8. Handoff for Buttons & Forms (Haya)

| Element | Text style | Icon |
|---|---|---|
| Button label | `type.label` | 20px (`icon.size.md`) |
| Input text | `type.body.default` | 20px inside the field |
| Input label | `type.label` | — |
| Placeholder | `type.body.default` in `neutral.text-secondary` | — |
| Helper text | `type.caption` in `neutral.text-secondary` | 16px |
| Error message | `type.caption` in `status.error` | 16px `error` icon |

## 9. Figma

The Figma file contains:
- **Cover** page
- **Typography** page — EN and AR text styles, type scale, text colors, and rules
- **Icons** page — 36 icon components, sizes, colors, and RTL rules
- DARB color variables (from 01-Branding) used for all text and icon colors

## 10. Screenshots

![Typography board] - 
![Icons board] - 

## 11. Approval Status

Proposed typography and icons – pending team review and approval.

## 12. Figma Link

[DARB Typography & Icons](https://www.figma.com/design/W0stvoEGQj49GDKzKn2mHF)
