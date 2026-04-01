# Mixtape Machine

Mixtape Machine is a shareable retro music page built around a Walkman-style player UI.

Paste a Spotify or SoundCloud link, load it into the page, and share the result as a themed mixtape link.

## What It Does

- Loads Spotify links for playlists, tracks, albums, artists, shows, and episodes
- Loads SoundCloud share links for tracks, playlists, and artist pages
- Shows the loaded title written directly on the Walkman body
- Opens the native share sheet on supported mobile browsers
- Falls back to copying the share link to the clipboard on desktop
- Keeps the Walkman player UI while styling the rest of the page with a chunky retro layout

## How It Works

The app is client-side only.

- `index.html` contains the full UI, styling, and behavior
- Spotify embeds use Spotify's standard embed URLs
- SoundCloud embeds use the SoundCloud player plus the SoundCloud Widget API
- Shared links are encoded into the `?playlist=` query parameter
- The last loaded link is saved in `localStorage`

## Usage

1. Open `index.html` in a browser.
2. Paste a Spotify or SoundCloud URL.
3. Click `Load Playlist`.
4. Press play on the Walkman.
5. Click `Share This Mixtape` to open the native share sheet or copy the share link.

## Local Preview

If you want to run it from a simple local server:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://127.0.0.1:8000/index.html
```

## Notes

- Some third-party embeds can behave differently across browsers and devices.
- SoundCloud is supported here because it is generally more reliable for shared embeds than YouTube in this kind of page.
- The repo ignores local tool folders like `.claude/` and `.playwright-mcp/`.
