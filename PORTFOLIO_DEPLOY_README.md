# Mayor — UGC Portfolio

Static portfolio site for Mayor (Mayowa Oladipo). Deploy on Render in 5 minutes.

## Files
- `index.html` — Main portfolio page (photo embedded, ~1.5MB)
- `rate_card.html` — Full rate card (linked from main page)
- `videos/` — Drop your spec ad MP4s here (see `videos/README.txt`)

## Deploy to Render

1. Go to https://render.com → sign up / log in
2. Click **New** → **Static Site**
3. Connect a GitHub repo OR drag-and-drop this folder
   - If using GitHub: push this folder to a new repo first
   - If using direct upload: zip this folder, upload zip
4. Settings:
   - **Build Command:** (leave empty)
   - **Publish Directory:** `.` (single dot — means "this folder")
5. Click **Create Static Site**
6. Render will give you a URL like `mayor-ugc.onrender.com`
7. Custom domain: in site settings → **Custom Domains** → add yours

## After deploy

- Open the URL on phone + laptop to test
- Print to PDF from `/rate_card.html` if a brand wants a downloadable copy
- Update content by editing files locally, then push to GitHub (Render auto-redeploys)

## Updating videos

See `videos/README.txt` for the exact swap pattern.

## Updating the day counter

Counter starts **Jan 1, 2026**. Auto-updates every day to "Day X / 365" via JavaScript in `index.html`. If you want to change the start date, edit this line near the bottom of `index.html`:

```js
var start = new Date('2026-01-01T00:00:00');
```
