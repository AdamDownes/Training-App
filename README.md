# Crux Training

A mobile-first, installable climbing training plan and progress log. It includes the September 2026 plan and can import future plans in the same spreadsheet layout.

## Put it on GitHub Pages

1. Create a new GitHub repository and upload every file and folder in this project.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions**. The included workflow publishes the app automatically.
4. When the action finishes, open the Pages address shown in the deployment. On iPhone use **Share → Add to Home Screen**; on Android use **Install app** from the browser menu.

All completions and training logs are stored in that browser on that device. Use **More → Export backup** before clearing browser data or changing phones.

## Updating the plan

- Recommended: in Google Sheets choose **File → Download → Microsoft Excel (.xlsx)**, then upload it in the app.
- A public Google Sheets link can also be pasted into the app. Google may block direct browser downloads in some configurations; the Excel upload remains the reliable fallback.

The importer expects the same broad structure as the supplied workbook: an `Overview` sheet with a `Date` row, plus sheets whose names contain `FB`, `warm`, and `SnC`.

## Local preview

Serve the folder with a small local server rather than opening `index.html` directly. For example: `python -m http.server 8080`.
