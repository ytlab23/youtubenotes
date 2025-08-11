# YouTube Timestamp Notes

A single-page app to take timestamped notes for any YouTube video. Notes are saved in your browser (localStorage) per video, and a library view shows your past videos.

## Deploy on GitHub Pages

1. **Create a new repository** on GitHub (any name, e.g. `youtube-timestamp-notes`).  
2. **Upload** the files from this folder to the repo root (`index.html`, `404.html`, `.nojekyll`, `README.md`, `LICENSE`).  
3. Go to **Settings → Pages**:  
   - **Source**: *Deploy from branch*  
   - **Branch**: `main` (or the default branch), **Folder**: `/root`  
4. Click **Save**. After a minute or two, your site will be live at:  
   `https://<your-username>.github.io/<your-repo>/`

> Tip: The favicon is embedded; no extra assets needed.

## Features

- Paste a YouTube URL or ID and load the video
- Add notes tied to timestamps; click a timestamp to seek
- Use the player's current time or type `hh:mm:ss`, `mm:ss`, `90`, `1m30s`
- Notes saved locally **per video**
- Library of your saved videos (thumbnail, note count, last updated)
- Import/Export JSON and Export CSV
- Mobile-friendly layout
- Keyboard: press **N** to grab current time into the note

## Local development

You can open `index.html` directly (`file://`). Some history functions are disabled in this mode for safety, but everything else works. For a local server, run for example:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/`.

## License

MIT — see `LICENSE`.
