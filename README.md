# JS ▸ PY Algo Flashcards — Fork & Deploy Guide

A mobile flashcard deck for JS/Python fundamentals, built for studying on the go before Codewars / LeetCode / HackerRank sessions. Fork it, deploy your own copy for free on GitHub Pages, and add it to your phone's home screen so it opens like a native app.

Your progress saves **on your own phone** — every person who deploys gets their own independent copy.

---

## Part 1 — Fork the repo

1. Go to the source repo: **https://github.com/maunahaole/algo-drills**
2. Click **Fork** (top-right). Leave the name as `algo-drills`.
3. Make sure **Copy the `main` branch only** is checked, then click **Create fork**.

You now have your own copy at `https://github.com/YOUR-USERNAME/algo-drills`.

> Keep the fork **Public** — free GitHub Pages only serves public repos. There are no secrets in this file, just study cards, so public is fine.

---

## Part 2 — Turn on GitHub Pages

1. On **your fork**, go to **Settings** (top bar) → **Pages** (left sidebar).
   - Direct link: `https://github.com/YOUR-USERNAME/algo-drills/settings/pages`
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Set **Branch** to `main` and folder to `/ (root)`, then click **Save**.
4. Wait ~1–2 minutes for the first build. Refresh the page — a green banner shows your live URL:

   ```
   https://YOUR-USERNAME.github.io/algo-drills/
   ```

If you hit the URL before the build finishes you'll get a 404 — just wait and refresh. You can watch the build under the repo's **Actions** tab.

---

## Part 3 — Add it to your phone

Open your live `github.io` URL on your phone first, then follow your platform.

### iPhone / iPad (Safari)

1. Open the URL in **Safari** (must be Safari, not Chrome — only Safari can install web apps on iOS).
2. Tap the **Share** button (square with an up arrow).
3. Scroll down and tap **Add to Home Screen**.
4. Name it (e.g. "Algo Drills") and tap **Add**.

It launches full-screen with no browser bars, and your progress persists on the device.

### Android (Chrome)

1. Open the URL in **Chrome**.
2. Tap the **⋮** menu (top-right).
3. Tap **Add to Home screen** (may appear as **Install app**).
4. Confirm **Add** / **Install**.

Same result — full-screen launch, progress saved locally.

---

## How to use it

- **Tap a card** to flip between question and answer.
- **GOT IT ✓** retires the card and saves your progress.
- **AGAIN** sends it to the back of the stack to see again.
- **Category tabs** at the top let you drill one topic (e.g. just Loops).
- **⇄** shuffles the current deck.
- **reset** (top-right) clears progress for the current category so you can run it fresh.

Keyboard shortcuts (if you open it on a laptop): `Space` flips, `1` = again, `2` = got it.

---

## Editing the cards (optional)

All cards live in the `DECK` array inside `index.html`. Each card looks like:

```js
{id:"x1", cat:"Loops", q:"Your question",
 a:"The answer. Wrap terms in [[double brackets]] for code styling.",
 js:"// optional JavaScript snippet",
 py:"# optional Python snippet",
 note:"optional green callout"}
```

To publish changes, commit and push to `main` — Pages redeploys automatically within a minute:

```bash
git add index.html
git commit -m "Update cards"
git push
```

---

*Built as a Code Platoon study aid. Fork freely, add your own cards, share your deck.*
