# NoticeBondhu
A Bangla-first notice helper by Zahirul Islam. Paste Bangla or English notice text, inspect candidate deadlines, dates, action lines, fee mentions and URLs, then maintain a personal checklist.

## Run
Open index.html in a modern browser. No build process, API key, external dependencies or backend. Use GitHub Pages for a consistent browser-storage origin.

## GitHub Pages
1. Create a public repository named NoticeBondhu.
2. Upload index.html, style.css, core.js, app.js, README.md and LICENSE to its root (not the ZIP).
3. Settings → Pages → Deploy from a branch → main → / (root) → Save.
4. Expected URL: https://iamzahirul.github.io/NoticeBondhu/
5. Leave Custom domain blank. Link this demo from your existing portfolio.

## Features
- Rule-based candidate extraction with original line references
- Bengali digit normalization and common full date patterns
- Deadline lines remain visible even without a recognized date
- User-reviewed action conversion into an editable task
- Checklist completion, deletion and optional user-chosen date
- Validated JSON backup / replacement restore
- Printable result and checklist
- Responsive layout and footer with creator, portfolio and GitHub links

## Limits and privacy
This is not an AI summarizer. It can miss dates, deadlines or actions and can flag irrelevant lines. It scans lines; separate lines may contain related context. It does not interpret ambiguous numeric dates, resolve relative dates, verify notice authenticity or send reminders. Always check the source text. Paste plain text only; PDF/image/OCR upload is not implemented.

Notice text and title are not persisted. Checklist tasks are stored only in this browser using localStorage. Browser data removal deletes tasks; back up regularly. Restore replaces all current tasks after confirmation. No cloud sync, encryption or multi-user accounts. External links open only when you click them. No service worker; offline reload is not implemented.

## Verification
Run `node tests.cjs` for extraction and backup validation checks. Browser visual/end-to-end verification was unavailable in the build environment; verify appearance and interactions in your browser before real use.

## Future improvements
PDF text extraction, additional date formats, export to calendar, offline reload support and bilingual interface.
