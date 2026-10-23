# Gather & Thrive website

Live site: https://sydhoeper.com/Gather-Thrive/

A small static website with no build step, dependencies, tracking, or JavaScript requirement. GitHub Pages publishes the root of `main`.

## Making changes

- `index.html`: homepage copy, sections, photos, contact details, and questions.
- `accessibility.html`: accessibility information and feedback contact.
- `styles.css`: shared design. Edit the variables under `:root` to change colors, typography, spacing, and borders throughout the site.
- `assets/`: the two meeting-room images supplied for this website. Replace them and update their descriptions and dimensions together.

Keep links relative so the site works under `/Gather-Thrive/` and on a future custom domain. No hosting migration is needed for a design change. Pull the latest `main` before editing; commit and push to publish.

## Content decisions

The two website drafts supplied were identical. The newer availability note is used instead of the older applications invitation. No donation link, event dates, fees, or booking form were supplied; none are invented. The user supplied info@gatherandthrivemt.org for public inquiries. Email and the supplied public PO box appear on both pages.

Only the supplied room photographs are published. The watermarked stock image, source documents, account credentials, and old hosting material are not part of this repository.

## Accessibility maintenance

Target: WCAG 2.2 AA and applicable Revised Section 508 web requirements (including WCAG 2.0 AA and parsing checks). See `ACCESSIBILITY.md` for verification scope and remaining review work.

After any design/content change, recheck contrast, keyboard operation, focus visibility, image alternatives, narrow layouts, browser zoom, and text spacing. Keep heading order meaningful, link names descriptive, and interactive targets at least 44 CSS pixels where practical. Do not disable browser zoom or remove focus outlines.

## Small design system

Five shared type roles live in `styles.css`: display (64px, 48px on mobile), section heading (32px), body (18px), secondary text (16px), and footer credit (12px). Subheadings use body size with heavier weight; introductory copy and addresses use body size. All sizes use rem units to respect browser preferences.

Spacing uses a shared 4 / 8 / 16 / 24 / 32 / 48 / 80px scale. Section spacing is 80px on desktop and 48px on mobile. Shared colors, typography, spacing, and radius are defined at the top of the stylesheet; both pages use the same system.
