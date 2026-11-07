# SIRE 2.0 Quick Reference (Chapters 2–10)

Searchable, offline-capable reference built from the OCIMF SIRE 2.0 Question Library v1.0 (Jan 2022).
Filter by chapter, vessel type, person responsible and remark status; mark questions Checked / Satisfactory / Follow up and add notes (saved on the device).

## Publish on GitHub Pages
1. Create a new GitHub repository (e.g. `sire2-quick-reference`).
2. Upload **all files in this folder** (keep the `icons` folder and the hidden `.github` folder) to the `main` branch.
3. In the repo go to **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Open the **Actions** tab and wait for "Deploy to GitHub Pages" to finish (about a minute).
5. Your app is live at `https://<your-username>.github.io/<repo-name>/`.

## Install on a phone
Open the link, then **Android/Chrome**: menu → *Install app*. **iPhone/Safari**: Share → *Add to Home Screen*. After the first visit it works offline.

## Files
- `index.html` – the app (all data embedded)
- `manifest.webmanifest`, `sw.js` – install and offline support
- `icons/` – skull app icon (SVG and PNG)
- `.github/workflows/pages.yml` – automatic deployment

Note: if you change `index.html`, change `CACHE='sire2-v1'` in `sw.js` to a new name so installed copies update.
The “person responsible” tags are suggestions derived from question wording and inspection location, not part of the OCIMF text. SIRE 2.0 content is © OCIMF; check their terms before sharing publicly.
