# Echo – hosting and publishing guide

Echo is a static web app. It needs no server code, no accounts and no database.
Folder contents: `index.html` (the game), `manifest.webmanifest` and `sw.js` (install + offline), three icons.

## 1. Put it online for everyone (free, about 2 minutes)
Pick one. Each gives you a public https link anyone can open on any phone.
- **Netlify Drop:** go to app.netlify.com/drop and drag this whole folder onto the page.
- **Cloudflare Pages:** create a project, choose "Direct upload", upload this folder.
- **GitHub Pages:** put these files in a repository, then Settings > Pages > deploy from the main branch.

It must be served over https for install and offline mode to work. Opening index.html straight from a file still plays fine, just without install.

## 2. How players install it
- **iPhone / iPad (Safari):** Share > Add to Home Screen.
- **Android (Chrome):** menu > Install app (or Add to Home Screen).
- **Desktop Chrome / Edge:** install icon in the address bar.
After the first visit it also works offline.

## 3. Put it in the App Store and Google Play (optional)
- **Easiest:** pwabuilder.com. Paste your hosted link and it produces Android (Play Store) and iOS packages.
- **More control:** wrap the folder with Capacitor (capacitorjs.com), which builds native iOS and Android projects.
- Needs a Google Play developer account and an Apple Developer Program account (both paid). Apple may ask for more than a plain web wrapper, so a few native touches (such as haptics) can help review.

## 4. Before you publish
- Scores, streaks and badges are saved on each player's own device (local storage). Nothing is collected or sent anywhere, so the privacy policy can say so.
- The game loads one Google Font (Fredoka) and falls back to the phone's own font if offline. To remove that external call, self-host the font file.
- Replace the icons with your own artwork any time (keep the same file names).
