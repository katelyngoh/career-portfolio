# Katie Goh — Career Portfolio

Personal career portfolio of Katie Goh, hosted free on GitHub Pages.

**Live site:** https://katelyngoh.github.io/career-portfolio/

It's a plain HTML + CSS site. There's no build step, no framework, and nothing to install: every file you see is exactly what gets published.

## What's in here

| File | What it is |
|---|---|
| `index.html` | Home page: intro, track record, case study cards, about, contact |
| `resume.html` | Resume (has a "Print / Save as PDF" button) |
| `gg-offroad.html` | GG Offroad case study |
| `behavioral-health-seo.html` | Healthgrades behavioral health SEO case study |
| `google-shopping.html` | Google Shopping / Merchant Center launch case study |
| `mention-watch.html` | Mention Watch (AI forum-listening agent) case study |
| `shopify-collective.html` | Shopify Collective retail channel case study |
| `syndicated-reviews.html` | Healthgrades syndicated reviews case study |
| `404.html` | Shown when someone visits a page that doesn't exist |
| `assets/css/style.css` | All colors, fonts, and layout for every page |
| `assets/img/` | Photos, logo, and work thumbnails |
| `.nojekyll` | Tells GitHub to publish the files as-is (leave it alone) |

## Turning the site on (one time)

1. In this repo on GitHub, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and folder to `/ (root)`, then click **Save**.
4. Wait 1–2 minutes and refresh. GitHub shows the live URL at the top of that page.

The site's address comes from the repository name: `katelyngoh/career-portfolio` publishes to `https://katelyngoh.github.io/career-portfolio/`. If you ever rename the repo, update the `https://katelyngoh.github.io/career-portfolio/` links in the `<head>` of each page and the `/career-portfolio/` paths in `404.html`.

## Making changes

**Easiest way (in the browser):**
1. Open the file on GitHub (for example `resume.html`).
2. Click the pencil icon (**Edit this file**).
3. Change the text between the tags — e.g. the words inside `<li>…</li>` or `<p>…</p>`. Leave the `<…>` tags themselves alone.
4. Click **Commit changes…**, write a short note like "Update resume dates", and commit to `main`.
5. The live site updates within a minute or two.

**With Claude:** start a Claude Code session with this repository selected and describe the change in plain English ("add a new job to the resume", "add a case study for X"). Claude edits the files, and you review and publish.

**Swapping an image:** upload a new file into `assets/img/` with the *same file name* (GitHub: **Add file → Upload files**), and it replaces the old one everywhere.

**After changing `assets/css/style.css`**, update the `?v=` date in the stylesheet link at the top of every `.html` file (e.g. `style.css?v=2026-11-03` → today's date). That makes visitors' browsers load the new styles right away instead of a saved old copy.

**Header, nav and footer** are repeated at the top and bottom of each `.html` file. If you change a nav link, change it in every page.

## Previewing locally (optional)

Open `index.html` directly in a browser, or run a tiny local server from this folder:

```bash
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Custom domain (optional, later)

To use something like `katiegoh.com`: buy the domain, go to **Settings → Pages → Custom domain**, enter it, and follow GitHub's DNS instructions. Then update the `https://katelyngoh.github.io/career-portfolio/` links in the `<head>` of each page (the `canonical` and `og:` lines) to the new domain, and change the `/career-portfolio/` paths in `404.html` back to `/`.
