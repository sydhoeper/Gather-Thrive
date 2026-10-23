# Accessibility review

Reviewed October 23, 2026. Target: WCAG 2.2 Level AA plus applicable Revised Section 508 web requirements, which incorporate WCAG 2.0 AA. This record is not a certification or complete conformance report.

## Scope

Homepage and accessibility page. Static HTML/CSS; no JavaScript required, third-party embeds, forms, media players, authentication, dragging, timed interactions, or automatic updates. Native HTML details controls provide the FAQ interaction.

## Completed checks

- axe-core 4.10.3 checks tagged WCAG 2 A/AA, WCAG 2.1 A/AA, WCAG 2.2 AA, and best practices: no violations or incomplete results in tested configurations.
- Both pages tested at 1280 CSS pixels and 320 CSS pixels, including increased text spacing and 200% root text size. No document-level horizontal overflow in tested configurations.
- Text spacing override: line height 1.5, paragraph spacing 2em, letter spacing .12em, word spacing .16em.
- Keyboard skip link is first focusable item, visible on focus, and transfers focus to main. Next Tab reaches the first main-content link.
- FAQ opens with Enter and closes with Space. Focus stays visible with a 3px outline.
- Navigation targets have at least 44px minimum height; the inline standards link uses the inline-text target-size exception.
- Descriptive image alternatives, page language, distinct titles, one H1 per page, meaningful heading order, landmarks, consistent navigation, and descriptive links inspected.
- No duplicate IDs, broken local fragment targets, or missing local resources found. HTML parsed successfully.
- Desktop and 320px layout visually inspected. No sticky overlays obscure focus. No animation or autoplay.
- Central color values pass automated text contrast checks. Footer credit uses scalable 12px text and the same high-contrast secondary text color.

## Remaining verification

- Complete criterion-by-criterion conformance review, including all applicable Revised Section 508 requirements.
- Screen reader testing with VoiceOver/Safari and NVDA/Firefox or Chrome; accessibility-tree inspection is not a replacement.
- Real browser 200% and 400% zoom across browsers. The 320px reflow and root text-size tests are useful proxies, not full browser zoom verification.
- Windows forced-color mode and mobile assistive technology checks.
- Testing with disabled users, including people with low vision and motor disabilities.
- Recheck external destinations separately; they are outside the scope of this site's review.

## Maintenance

Recheck after content, colors, fonts, navigation, or interactions change. Keep alternative text meaningful; do not embed essential copy in images. New forms and media need their own accessibility review. Public feedback: info@gatherandthrivemt.org.

References:
- https://www.w3.org/TR/WCAG22/
- https://www.section508.gov/test/websites/
