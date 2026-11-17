# The Road to Great Falls — 2027

Static, mobile-friendly itinerary website for GitHub Pages.

## Publish
1. Create a public GitHub repository named `great-falls-rally-2027`.
2. Upload all files and folders from this project to the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)` and save.
4. Open `https://YOUR-USERNAME.github.io/great-falls-rally-2027/` after deployment.

## Update the itinerary
- Edit `data/itinerary.json` directly in GitHub, commit and wait for Pages to republish.
- Or use **Edit / Export** on the website, **Apply changes to preview**, then **Download updated JSON** and replace `data/itinerary.json` in the repository. Browser edits alone do not publish changes.
- TXT is generated from the current itinerary in the browser.
- Add only verified GPX files under `routes/` and set the corresponding `gpx` field to a relative path, e.g. `routes/day-01.gpx`.
- Custom map links can be added to `mapUrl`; if empty, the site builds a Google Maps directions link from `stops`. Google Maps links are not verified GPX tracks.

## Preview locally
Run `python3 -m http.server 8000` from the project folder and open `http://localhost:8000/`. Direct `file://` loading can block JSON fetches.

## Privacy
GitHub Pages is public. Do not publish rider emergency logs, personal phone numbers, medical information or insurance details.
