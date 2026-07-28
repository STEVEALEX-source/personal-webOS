# personal-webOS

hey! welcome to personal-webOS, a tiny desktop environment that runs entirely inside your browser. 

i built this whole thing using just vanilla HTML, CSS, and JS. no massive frameworks, no React, no npm installs, and no backend servers. literally just one HTML file that does everything.

---

## cool stuff it can do

- window management: you can drag, resize, maximize, minimize, and close windows (it even has cool genie/fade animations when you open them).
- live wallpapers: built 4 canvas wallpapers from scratch (Aurora, Nebula, Orbs, and Circuit). zero images downloaded from the web, all drawn with math in JS!
- actual working apps:
  - Files: browse your saved stuff.
  - Notepad: type notes and save them.
  - Terminal: run basic commands.
  - Browser: embed pages inside windows.
  - Settings: customize accent colors, toggle wallpapers, and sound effects.
- file saving: anything you write in notepad stays there even if you refresh, thanks to localStorage.
- sound effects: generated UI sounds using the browser's AudioContext (no .mp3 files needed).
- desktop features: start menu, taskbar tabs, right-click context menu, live clock, and notifications.

---

## tech used

- HTML5 (semantic structure & inline SVGs for the icons)
- CSS3 (glassmorphism effects, flexbox/grid, keyframe animations)
- Vanilla JavaScript (DOM manipulation, canvas animations, drag/resize logic)
- Web Audio API (synthesizing UI sound blips)

---

## how to run it

since it's literally just standard web tech, you don't need Node.js or any local server stuff.

1. clone the repo:
   ```bash
   git clone [https://github.com/STEVEALEX-source/personal-webOS.git](https://github.com/STEVEALEX-source/personal-webOS.git)
