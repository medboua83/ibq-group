# Design QA — IBQ GROUP

Source visual truth: C:/Users/ASUS/.codex/generated_images/01a1e4bf-c07b-7f52-95f8-d1f2559b6597/exec-1c7b08a6-37e6-49aa-a33b-71651daf2a4a.png
Implementation: qa/desktop-final.png
Full comparison: qa/comparison-final-2.png
Viewport: 1440 × 1000 CSS px; source 1122 × 1402 px. Rendered full-page content 1424 px wide (scrollbar excluded), normalized proportionally to 1122 px in comparison. State: home, dialog closed.

## Findings and history
- Initial P2: expertise typography was undersized relative to the reference. Increased it, then comparison revealed an unwanted wrap of the LED heading at 49px. Restored 46px; final capture confirms single-line heading, three balanced rows and matching hierarchy.
- Initial P2: mobile line break hid the space between headline sentences. Added explicit space and reduced mobile heading to 40px. Browser DOM confirmed corrected text.
- No remaining actionable P0/P1/P2 findings.

## Required fidelity surfaces
- Typography: Manrope matches geometric heavy sans direction; Barlow Condensed for the wordmark extension. Headline wraps in two desktop lines. Minor width differences in supporting headings are P3.
- Spacing: wide hero, equal expertise columns, three separated rows and bottom CTA preserved. Mobile stacks cleanly without horizontal overflow (390px viewport, 375px document width excluding scrollbar).
- Colors: charcoal hero, warm off-white body, orange actions and fine separators follow source.
- Imagery: four individually generated photos match reference subjects and art direction. Official IBQ logo used instead of mockup's invented globe. Gold raster badge preserved; slightly smaller visible badge is P3.
- Copy: headline, descriptions and CTA match the selected concept. Caption corrected to professional integration. Added small email footer and dialog to support the main conversion path.

## Focused evidence
Hero text and first expertise were inspected in the 1440px browser viewport at full size; full-view comparison retains readable headings. Mobile screenshot: qa/mobile.png. Form inspected in browser: required fields, selection, prepared state and encoded mailto body all verified. Email was not sent. Menu open/close and expertise anchor verified at 390 × 844. All six images loaded. Console inspected: no errors, only Vite/React development information.

## Accepted limitations
Photo assets are illustrative generated imagery, not documented IBQ projects. Email submission depends on the visitor's mail client. External font service and actual email sending were not independently tested.

## Implementation checklist
- [x] Responsive page, navigation and contact dialog
- [x] Reference comparison and post-fix captures
- [x] Primary conversion flow tested without transmission

final result: passed
