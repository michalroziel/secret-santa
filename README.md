# Secret Santa 🎅

A tiny Secret Santa site. Add everyone's names and draw. Then send each person their own private link that reveals who they're buying a gift for.

No sign-ups and no server. Nothing is stored online.

## How it works

1. **The organizer** opens the site and adds everyone's names (including their own).
   - **Keep apart** (optional): pairs who shouldn't draw each other, like couples.
   - **Details** (optional): budget, when & where, and a short note. Everyone sees these.
2. Click **Draw names**. The draw happens in the browser. Nobody gets themselves, and the keep-apart rules are always respected. The organizer never sees who got whom.
3. Each person gets a **Copy link** button for their personal link, ready to paste into a chat or a browser. On phones there's also a **Share** button that sends it with a short message.
4. Each friend opens their link, taps the gift, and sees their match. 🎁

The organizer page remembers the drawn links in that browser, so you can come back later to finish sending them.

### Good to know

- Each match is stored inside that person's link, after the `#`. Browsers never send that part to the server, so GitHub never sees it.
- The match is **scrambled, not encrypted**. Nobody can read it at a glance, but a determined techie could decode their own link. Fine among friends.
- If you draw again, everyone needs their new link. The old links won't match the new draw.

## Put it online with GitHub Pages

1. Merge this into the `main` branch.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Then pick branch **`main`** and folder **`/ (root)`**, and click **Save**.
4. Wait a minute or two. The site will be live at:
   **https://michalroziel.github.io/secret-santa/**

> On a free GitHub account the repository must be **public** for Pages to work. The repo only contains the code. Your friends' names never end up in it.

## Try it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.
