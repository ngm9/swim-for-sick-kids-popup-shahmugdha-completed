# Nerdium Frontend Screening — Swim For Sick Kids Popup

## Task Overview

Nerdium is hiring frontend developers and uses a practical, design-replication challenge as part of its screening process. In this task you will complete a real-world popup component built for the **Swim For Sick Kids** charity — a registration-prompt overlay that encourages visitors to sign up and claim a free swimming cap. The popup was originally designed by the agency Designerds and must appear, behave, and look exactly as specified below. Your job is to wire up the timing, dismissal, call-to-action redirect, and visual styling so the finished result matches the design reference.

---

## Design Reference
This is the reference image for the design you need to replicate: https://drive.google.com/file/d/1g-SGZ4AqnBF-2vjGlytozk5Dlt4FGJYy/view

---

## Objectives

  - When the page first loads the popup is not visible. 5 seconds after the page finishes loading the popup appears centred on the page with the rest of the page dimmed behind it.
  - Clicking the close icon at the top-right of the popup dismisses both the popup and the dim backdrop, and the popup does not reappear during that page session.
  - Clicking the SIGN UP NOW! button opens https://designerds.com.au in a new browser tab.
  - The popup's appearance — colours, rounded corners, typography, button, close icon, centred swim-cap image, and dimmed backdrop — visually matches the design reference linked above.
  - The implementation uses only plain HTML, CSS, and JavaScript. No frameworks, no build tooling.
---

## Helpful Tips

- Consider how CSS positioning techniques can be used to pin an overlay to the full viewport and centre a floating card both horizontally and vertically, regardless of page scroll position.
- Think about a built-in browser mechanism that runs a callback function once after a specified number of milliseconds — this is the natural tool for the 5-second delay.
- Explore how a single JavaScript function can be responsible for changing the visibility state of multiple elements on the page at the same time when a user clicks a button.
- Review how the `<a>` element's attributes control both the destination URL and whether the browser opens it in the current tab or a new one, and how JavaScript event handling can complement or override that behaviour.

---

## How to Verify

- Open `index.html` directly in a browser (no server required). Confirm the popup is **not visible** on initial load.
- Wait 5 seconds without interacting with the page — the popup and its backdrop must appear automatically at the 5-second mark, not before and not significantly after.
- Click the × close icon at the top-right of the popup. Both the popup and the backdrop must disappear immediately and must not reappear for the rest of that page session.
- Click the **SIGN UP NOW!** button while the popup is visible — your browser must open a **new tab** navigating to `https://designerds.com.au`; the original tab must remain on your local page.
- Compare your result visually against the embedded design reference above: dark navy background, yellow headline and button, white body text, rounded corners on the popup and button, circular product image, and a semi-transparent dark backdrop dimming the rest of the page.
