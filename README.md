# WebOS

a fake desktop os that runs entirely in your browser. no backend, no build tools, no npm install, its literally just one html file. open it and it boots up like an actual computer lol

live demo: just open `index.html` in your browser, thats it

![status](https://img.shields.io/badge/status-actually%20works-brightgreen)

## why

wanted to see if i could build something that felt like a real desktop (windows, taskbar, icons, wallpapers that move) using nothing but html/css/vanilla js. no react, no frameworks, no external images or audio files. everything you see is either drawn on a `<canvas>` or built with plain divs.

## features

- **boot screen** with a fake loading bar so it feels like an actual startup
- **draggable + resizable windows** with minimize / maximize / close, just like a real os
- **taskbar** that tracks open apps, click a tab to bring that window back up
- **start menu** for launching apps without hunting for the icon
- **right click menu** on the desktop (new file, refresh icons, change wallpaper, about)
- **4 live wallpapers**, all canvas animations, no video/gif files:
  - Aurora — drifting light ribbons
  - Nebula — twinkling stars + drifting color clouds
  - Orbs — glowing blobs bouncing around
  - Circuit — pulsing signal grid
- **apps:**
  - Notepad — write + save text files
  - File Manager — browse saved files
  - Terminal — `help`, `ls`, `cat <file>`, `live <wallpaper>`, `clear`
  - Browser — loads any url in an iframe
  - Settings — change wallpaper, accent color, toggle sound/chime
- **saves everything to localStorage** so your files and settings stick around after a refresh
- small ui sound effects (generated with the Web Audio API, not mp3s)
- 5 accent colors that reskin the whole ui instantly

## how to run it

no install needed, its one file.

1. download `index.html`
2. double click it, or drag it into your browser
3. thats literally it

if you want to serve it properly (some browsers are picky about local files):

```bash
python3 -m http.server
# then go to localhost:8000
```

## built with

- html
- css (canvas-drawn wallpapers, css vars for theming, no external stylesheets)
- vanilla javascript (no frameworks, no libraries)
- localStorage for saving files/settings
- Web Audio API for the little click sounds

## known issues / stuff i might fix later

- terminal commands are pretty basic, could add more
- no real "install" or download support in the fake browser, its just an iframe
- windows dont snap to edges yet
- probably some edge cases with resizing super small

## credits

made by Rizz

repo: [github.com/STEVEALEX-source/personal-webOS](https://github.com/STEVEALEX-source/personal-webOS)

if you use any of this or build on top of it, a shoutout would be cool but not required :)
