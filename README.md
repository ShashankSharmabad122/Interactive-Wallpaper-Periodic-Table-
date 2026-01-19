**Periodic Table — Interactive Wallpaper**

- **What:** A responsive, interactive periodic-table webpage you can use as a live/interactive wallpaper on Windows.
- **Maker:** SHASHANK

**Files**
- **Index & styles:** [live/index.html](live/index.html), [live/style.css](live/style.css)
- **Restored wallpaper page:** [live/wallpaper.html](live/wallpaper.html)

**Quick usage (Lively)**
1. Open Lively Wallpaper.
2. Click the "+" (Add) button → choose "Add a new wallpaper from file".
3. Select the file: [live/wallpaper.html](live/wallpaper.html) (or [live/index.html](live/index.html)).
4. Set it as your wallpaper. Interaction (click/hover) will work when selected.

**Quick usage (Wallpaper Engine)**
1. Open Wallpaper Engine (Steam).
2. Click "Create Wallpaper" → "Create Web Wallpaper (local)".
3. Point to [live/index.html](live/index.html) or to the folder `live/` and choose the HTML entry file.
4. Adjust resolution/quality and save. Mark it as interactive if prompted.

**If local files fail to load (CORS / local resource issues)**
Some wallpaper engines or browsers block local file access. Serve files with a tiny local web server and point the wallpaper to `http://localhost:3000/live/index.html` (or the offered port).

Quick server commands (run from the workspace folder `C:\Users\shashank\live`):

PowerShell (Python 3):
```powershell
python -m http.server 3000
```

Node (if you have http-server installed):
```bash
npx http-server -p 3000
```

Then point Lively/Wallpaper Engine to:
- http://localhost:3000/live/wallpaper.html  or
- http://localhost:3000/live/index.html

**Make a fully self-contained single file**
If you prefer one self-contained file (single HTML with inlined CSS), I can generate `wallpaper.full.html` that embeds `style.css` and `index.html` into one file for easier import into wallpaper tools. Tell me and I'll create it.

**Customizing colors / theme**
- Edit the CSS variables in `:root` inside [live/style.css](live/style.css) (or in the single-file if you request it) to change colors quickly. Look for `--palette-bg` and `--palette-text`.

**Troubleshooting**
- If the wallpaper shows CSS text or the page looks blank: open the file in a regular browser tab (Edge/Chrome) to inspect console errors; message me the screenshot and I will fix it.
- If elements are very small or overflow: try resizing or run a local server and open `index.html` directly in the browser to check responsive behavior.

**Credits**
- Maker: SHASHANK
