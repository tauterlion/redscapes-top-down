# Redscapes Laboratory — V1.3

Standalone version of the current prototype.

## Run

Open `index.html` in a browser, click the game once, and use the arrow keys.

For local asset loading, a tiny local server is safer than opening the file directly:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Asset folders

- `assets/audio/` — put `picking-up-paper.mp3` here.
- `assets/documents/` — intended location for `RS_ARCHIVE_NOTE_01.pdf`.
- `assets/sprites/` — reserved for future player/object sprites.

The current document viewer still uses the built-in placeholder document UI. The real PDF path is already represented in `game.js`, so we can wire the viewer to the actual PDF later.


V1.7 note: the archive document now opens as a transparent PNG overlay at assets/documents/RS_ARCHIVE_NOTE_01.png instead of a PDF-style window.

V1.8 note: the black figure now stands inside the center Containment enclosure. Add `assets/audio/heartbeat.mp3`; it loops after the player's first interaction and rises from silent to a maximum volume of 50% as the player approaches the figure.