# Frederick Sister Cities Association — Website

Modern website for the Frederick Sister Cities Association (FSCA), connecting
Frederick, Maryland with its German sister cities of **Schifferstadt** and
**Mörzheim** since 1982.

Site: https://fredericksistercities.org

## What's in this repo

| File | Purpose |
|------|---------|
| `index.html` | **The site.** A single, self-contained file — fonts, styles, logo, and all seven pages are inlined. Works offline and can be served as-is. |
| `src/Frederick Sister Cities.dc.html` | Editable source (a Design Component). Edit this, then re-bundle to regenerate `index.html`. |
| `src/support.js` | Runtime that the source file depends on. |
| `src/assets/fsca-logo.png` | Association logo. |

## Pages

Home · About · Events · Get Involved (membership / host / donate) ·
Gallery · Newsletters · Contact + Board directory.

## Publishing with GitHub Pages

1. Repo **Settings → Pages**.
2. Under **Build and deployment**, set **Source: Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Save.
4. Your site goes live at `https://ynkeefn62.github.io/frederick-sister-cities/`
   (`index.html` is served automatically).
5. To use **fredericksistercities.org**, add a `CNAME` file containing that
   domain and point the domain's DNS at GitHub Pages.

## Still to do (placeholders in the design)

- Swap `[ photo: … ]` placeholders for real photos.
- Fill in actual board member names and current event / newsletter dates.
- Confirm the contact email and mailing address.
- Wire the membership, donation, and contact forms to a real service
  (email, payment, or a form provider). They are front-end mockups right now.

---
An affiliate of the Frederick County Landmarks Foundation (FCLF). 501(c)(3).
