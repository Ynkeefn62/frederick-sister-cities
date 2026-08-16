# Frederick Sister Cities Association — Website

Website for the Frederick Sister Cities Association (FSCA), connecting
Frederick, Maryland with its German sister cities of **Schifferstadt** and
**Mörzheim** since 1982.

Site: https://fredericksistercities.org

## What's in this repo

| Path | Purpose |
|------|---------|
| `index.html` | **The site.** A single, self-contained, hand-authored HTML/CSS/JS file — no build step, no bundler. Responsive from phone to desktop. Edit it directly. |
| `assets/` | Images and the newsletter PDF. |
| `favicons/` | Favicon set (16–512px, apple-touch-icon, .ico) generated from the FSCA logo. |
| `site.webmanifest` | Lets the icon be used as an Android/Chrome home-screen icon. |

## Pages

Home · About · Events · Get Involved (membership / host / donate) ·
Gallery · Newsletters · Contact + Board directory.

Navigation is a simple hash router (`#about`, `#contact`, etc.) implemented
in plain JavaScript at the bottom of `index.html` — no framework or build
step required. To add or edit a page, find its `<div class="page" id="page-...">`
block and edit the HTML directly.

## Mobile layout

Responsive breakpoints are defined in the `<style>` block in `index.html`:
- **≤900px**: two-column sections collapse to one column.
- **≤780px**: the top nav collapses into a hamburger menu (`#hamburgerBtn` /
  `#mobilePanel`).
- **≤480px**: hero type and buttons scale down further for small phones.

## Favicon / search engine icon

`index.html` links a full favicon set (16, 32, 48, 96, 192, 512px, plus a
180px apple-touch-icon and a legacy `.ico`) generated from `assets/fsca-logo.png`.
Google and other search engines pick up the icon automatically from the
`<link rel="icon">` tags on the homepage the next time they crawl the site —
there's no separate submission step, but it can take some time to appear in
search results after a fresh deploy.

## Publishing with GitHub Pages

1. Repo **Settings → Pages**.
2. Under **Build and deployment**, set **Source: Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Save.
4. Your site goes live at `https://ynkeefn62.github.io/frederick-sister-cities/`
   (`index.html` is served automatically).
5. A `CNAME` file containing `fredericksistercities.org` should already be
   in the repo root — that's what maps the custom domain to this site.

## Still to do (placeholders in the design)

- Fill in actual board member names and current event / newsletter dates.
- Confirm the contact email and mailing address.
- Wire the membership, donation, and contact forms to a real service —
  they currently open the visitor's email client via `mailto:` links rather
  than submitting to a form backend or payment processor.
- Add real gallery photos (Gallery page currently shows a placeholder).

---
An affiliate of the Frederick County Landmarks Foundation (FCLF). 501(c)(3).
