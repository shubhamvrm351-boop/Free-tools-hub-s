# ToolBox – free browser-based tools (MVP, Stage 3)

One file: `index.html`. No build step, no server, no paid services, no secrets.
Files you process never leave the visitor's device.

## What works
Resume + cover letter builder (live preview, PDF via print), Merge PDF, JPG/PNG to PDF,
Extract/Delete/Rotate PDF pages, Image resize/compress/convert (JPG, PNG, WebP),
Word counter, Case converter, Duplicate-line remover, Password generator,
Age calculator, Date calculator, QR generator.

## Not built yet (shown as "Soon")
Compress PDF, PDF to JPG, Image crop, PDF to Word / Word to PDF (needs a paid server for decent quality),
payments, admin dashboard, SEO pages, privacy/terms pages.

## Limits
- 25 MB per file. Very large files can crash a phone browser.
- Needs internet for two libraries (pdf-lib, qrcodejs) loaded from cdnjs.
- Resume PDF uses the phone's print dialog ("Save as PDF").
- Password-protected PDFs are rejected with an error, not unlocked.
- Not yet tested across many phones. Report anything that fails.

## Deploy from Android (free): Cloudflare Pages
1. Download this ZIP and keep it as a ZIP file.
2. In Chrome, open dash.cloudflare.com, create a free account, verify your email.
3. Go to Workers & Pages > Create > Pages > Upload assets (Direct Upload).
4. Name the project (becomes yourname.pages.dev), upload the ZIP or the extracted `index.html`, tap Deploy.
5. Open the .pages.dev link. To update later, create a new deployment with the new file.
(Cloudflare's menus change sometimes; look for "Pages" and "Direct Upload".)

## Alternative: GitHub Pages
1. Create a free account at github.com. In Chrome menu, turn on "Desktop site".
2. New repository, name it `toolbox`, set Public, create.
3. "Add file" > "Upload files", choose `index.html`, commit.
4. Settings > Pages > Source: Deploy from a branch > main > / (root) > Save.
5. After a minute the site is at https://YOURNAME.github.io/toolbox/
