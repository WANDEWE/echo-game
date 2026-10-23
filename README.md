# Echo 🧠

A simple, free brain-training game for all ages that runs in any phone
browser and installs to the home screen like an app.

**Play it:** https://preeminent-bavarois-ebef37.netlify.appss

## Modes
- **Classic:** watch the tile pattern, then repeat it in order.
- **Reverse:** repeat the pattern backwards.
- **Daily:** the same pattern for every player each day.
- **Number Flash:** memorise a number that flashes briefly, then type it.
- **Quick Sums:** mental arithmetic against a timer that gets harder as you go.

## Features
- Three speeds: Calm, Normal and Quick
- Three lives per game
- Daily streaks and unlockable badges
- Shapes as well as colours on the tiles, for colour-blind players
- Sound and vibration feedback, with sound switchable off
- Light and dark themes that follow the phone's setting
- Works offline as a Progressive Web App
- No accounts, no ads and no tracking. Scores stay on the player's device.

## Tech
A single static page in plain HTML, CSS and JavaScript, with a web manifest
and a service worker for install and offline support. No build step and no
dependencies. To run it locally, serve the folder with any static server,
for example `python3 -m http.server`, and open it in a browser.


