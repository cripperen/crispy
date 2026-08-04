Put your .mp3 files in this folder.

Then open index.html and find the SONGS array near the top of the
<script> section. Add one line per song, for example:

  const SONGS = [
    { file: "Sunset Drive.mp3", title: "Sunset Drive", artist: "Nova" },
    { file: "lofi-rain.mp3" },
  ];

You only need "file" — title/artist are optional and will be guessed
from the filename if left out.

Tip: if you run a local server from the project folder, e.g.

  python3 -m http.server

...and open http://localhost:8000, you can leave SONGS empty and
Spindle will try to auto-detect the mp3 files in this folder for you.
This auto-detect trick does NOT work if you just double-click
index.html to open it directly (browsers block that for local files).
