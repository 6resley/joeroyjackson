# joeroyjackson.com

The website for blues guitarist Joe Roy Jackson: a scroll-driven 3D Stratocaster, the *Brothers* EP player, photos, shows, press kit and booking.

## What's here

| Path | What it is |
| --- | --- |
| `index.html` | The whole site (styles and scripts are inline) |
| `assets/guitar.glb` | The 3D guitar model, loaded by the page |
| `music/` | The five *Brothers* tracks and the EP cover |
| `photos/` | Cover photo and the gallery |
| `guitar-still.webp` | Still image shown on devices that can't run 3D |
| `amp-panel*.webp` | The Vibro-King panel between the cover and the guitar |
| `share.jpg` | Link-preview image (texts, Facebook, Instagram, X) |
| `apple-touch-icon.png` | Home-screen icon |
| `404.html` | Friendly "page not found" page that sends visitors back home |
| `robots.txt`, `sitemap.xml` | Help search engines find and index the site |
| `CNAME` | Tells GitHub Pages the site lives at joeroyjackson.com |

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

- The mailing list sign-up sends emails to Joe's Kit form (`LIST_ENDPOINT` in `index.html`). Kit emails each new subscriber a confirmation link; manage the list at kit.com.
- Optional: to have booking requests arrive without the visitor's email app, set `BOOK_ENDPOINT` in `index.html` to a form service address (e.g. Formspree). Until then the booking form opens a neatly laid-out, pre-filled email to Joe.

## Handy extras

- **Share a song:** every track has a share button. Links look like `joeroyjackson.com/#song-brothers` and open the page at the music with that song ready.
- **Keyboard:** space plays and pauses, arrow and Page keys move between sections, Home and End jump to the start and to booking.
- **Inspect the guitar:** at the end of the page, a button lets visitors spin and zoom the guitar.
