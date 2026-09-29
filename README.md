# Chordsmith Studio: publish it on GitHub Pages

These files make Chordsmith a website that people can also **install like an app** on Android, iPhone and computers. Once it's installed, it works offline. No build step and no app store are needed.

## What's in here

| File | What it does |
|---|---|
| `index.html` | The app |
| `manifest.json` | Tells phones the app's name, icon and colours, so it can be installed |
| `sw.js` | The offline helper: saves the app on the device after the first visit |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | App icons for Android, iPhone and desktop |
| `screen-1/2/3.png` | Screenshots shown in the install prompt on Android |
| `feature-graphic.png` | Preview image when you share the link on WhatsApp or social media |
| `privacy.html` | Privacy policy, linked at the bottom of the app |

All the files sit in one folder with no sub-folders, so you can upload everything from a phone.

## Step 1: Create the repository (3 min)

1. Sign in at **github.com** (create a free account if needed). Your username becomes part of the link.
2. Tap **+ → New repository**.
3. Name it `chordsmith` (or anything you like; this becomes part of the link).
4. Choose **Public**. Free GitHub Pages needs a public repository.
5. Tick **Add a README file**, then tap **Create repository**.

## Step 2: Upload the files (3 min)

1. Unzip the package on your phone or computer.
2. In the repository, tap **Add file → Upload files**.
3. Select **all** the files in the folder and upload them.
4. Tap **Commit changes**.

If GitHub asks whether to replace the existing `README.md`, say yes.

## Step 3: Turn on GitHub Pages (1 min)

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, set *Source* to **Deploy from a branch**.
3. Set *Branch* to **main** with folder **/ (root)**, then tap **Save**.
4. Wait 1–2 minutes and refresh. The page shows your link:

   `https://YOUR-USERNAME.github.io/chordsmith/`

## Step 4: Check it and install it

Open the link on your phone:

- **Android (Chrome):** tap **Install app** at the top of Chordsmith, or ⋮ → **Install app** / **Add to Home screen**.
- **iPhone (Safari):** tap **Share → Add to Home Screen**.
- **Computer (Chrome/Edge):** click the install icon in the address bar.

Then test the offline mode: turn on airplane mode and open Chordsmith from the home screen. It should still work, including sound, your songs, and the Hindi and Telugu text.

## Updating the app later

1. Upload the new `index.html` to the repository, replacing the old one.
2. People get the new version the next time they open the app while online.
3. If you also change icons or other files, open `sw.js` on GitHub (tap the pencil icon), change `chordsmith-v1` to `chordsmith-v2` (then v3, and so on), and commit. This refreshes everything that was saved on people's phones.

## Good to know

- **Where songs are saved:** in each person's browser on their own device. Songs made in the browser and in the installed app on the same phone are shared. They don't sync between different devices.
- **Code visibility:** the repository is public, so anyone can see the code. Your signing key and personal files are **not** part of this package; never upload them.
- **Custom domain (optional):** you can use a domain like `chordsmith.in` later, in **Settings → Pages → Custom domain**.
- **Google Play later:** this link works as your privacy-policy and website link if you publish on the Play Store. The earlier Android package and signing key still work for that.
