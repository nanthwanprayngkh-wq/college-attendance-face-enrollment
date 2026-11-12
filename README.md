# College Attendance face enrollment page

This folder contains the static browser page intended for GitHub Pages hosting.

## Files

- `index.html` is copied from the browser-based face enrollment camera page.
- No student roster, face template, API key, or student image belongs in this repository.

## Integration

The Apps Script `FaceBridge.html` must open this GitHub Pages origin and accept messages only from that exact origin. The camera page sends data to the Apps Script bridge through `window.opener`; it does not write to Google Sheets directly. Face embeddings are intended to be stored only by Apps Script in the existing `FaceDB` sheet after the workbook's sharing access is restricted.

Set the repository's GitHub Pages source to the root of the default branch and enforce HTTPS before sharing the page URL.
