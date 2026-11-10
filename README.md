# Copyright Free Sadaqah

A static website ready for GitHub Pages.

## Publish on GitHub
1. Create a public repository (for example `copyright-free-sadaqah`).
2. Upload `index.html`, `logo.png`, and the complete `Surah` folder to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site.

## Adding more MP3 files later
Upload each MP3 into the exact `Surah` folder. Then add its entry to the `tracks` array near the bottom of `index.html`, using this format:
`{"number": 2, "name": "Baqarah", "file": "2. Surah Baqarah.mp3"}`

Keep the filename in the array exactly identical to the uploaded filename. GitHub Pages filenames and folder names are case-sensitive.

The Listen and Download links use relative paths (`Surah/<filename>`), so they work on a GitHub Pages project site without hardcoding a repository URL.
