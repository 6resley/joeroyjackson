# joeroyjackson.com

The website for blues guitarist Joe Roy Jackson: a scroll-driven 3D Stratocaster, the *Brothers* EP player, photos, shows, press kit and booking.

## What's here

| Path | What it is |
| --- | --- |
| `index.html` | The whole site (styles and scripts are inline) |
| `assets/guitar.glb` | The 3D guitar model, loaded by the page |
| `music/` | The five *Brothers* tracks and the EP cover |
| `photos/` | Cover photo and the gallery |
| `videos/` | Video thumbnails |
| `guitar-still.webp` | Still image shown on devices that can't run 3D |
| `amp-panel*.webp` | The Vibro-King panel between the cover and the guitar |
| `share.jpg` | Link-preview image (texts, Facebook, Instagram, X) |
| `apple-touch-icon.png` | Home-screen icon |

The page needs to be served over http(s); opening `index.html` straight from disk won't load the 3D model.

## Publishing with GitHub Pages (free)

1. In this repository on GitHub: **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick the branch with these files and the `/ (root)` folder, then **Save**.
3. After a minute the site is live at the address GitHub shows.

### Using joeroyjackson.com

1. In **Settings → Pages → Custom domain**, enter `joeroyjackson.com` and save.
2. At your domain registrar, add the DNS records GitHub lists (four `A` records for the bare domain, a `CNAME` for `www`).
3. Once the check passes, tick **Enforce HTTPS**.

## Before launch

- Replace the four `SITE_URL` placeholders in the `<head>` of `index.html` with the real address (e.g. `joeroyjackson.com`) so link previews work.
- To connect the mailing list, set `LIST_ENDPOINT` in `index.html` (search for it) to your list service's form address. Until then the Join button opens a pre-filled email to Joe.
