# horizon-mep-site

This is a small static website repository designed to be hosted on **GitHub Pages** and embedded into **Google Sites** pages.

## Structure
- `index.html` — Home (embed in Google Sites Home page)
- `services.html` — Services index (embed in Services page)
- `mechanical.html` — Mechanical subpage
- `electrical.html` — Electrical subpage
- `plumbing.html` — Plumbing subpage
- `fire.html` — Fire Protection & Fire Alarm subpage
- `projects.html` — Projects gallery
- `about.html` — About Us
- `contact.html` — Contact page
- `request-quote.html` — Embeds the Google Form (replace placeholder)

## Before publishing (important)
1. Replace placeholders in HTML files:
   - `GS_HOME_URL`, `GS_SERVICES_URL`, `GS_PROJECTS_URL`, `GS_ABOUT_URL`, `GS_CONTACT_URL`, `GS_QUOTE_URL`, `GS_MECHANICAL_URL`, `GS_ELECTRICAL_URL`, `GS_PLUMBING_URL`, `GS_FIRE_URL`
     with the **published Google Sites page URLs** (for example: `https://sites.google.com/view/horizonmep/home`).
   - `GOOGLE_FORM_EMBED_URL` in `request-quote.html` with your Google Form embed URL (use the `embedded=true` form link).

2. Add your real contact details (email, phone, office location) in `contact.html` and footer areas.

## How to publish
1. Create a new GitHub repository (public).
2. Upload all files and the `logo.png` image.
3. In the repository settings -> Pages, enable GitHub Pages from the `main` branch.
4. After publishing, you'll get URLs like:
   `https://<username>.github.io/<repo>/mechanical.html`

## How to embed into Google Sites
1. Create corresponding pages in Google Sites (Home, Services, Mechanical, etc.) and publish the site.
2. Copy the published Google Sites page URL for each page.
3. Replace `GS_*_URL` placeholders in the HTML files with the Google Sites page URLs, then push changes to GitHub.
4. In Google Sites, edit the page -> Insert -> Embed -> By URL -> paste the GitHub Pages page URL (e.g., `https://<username>.github.io/<repo>/mechanical.html`).
5. Use `target="_top"` links in the embedded pages to navigate the parent Google Sites pages.

## Notes
- Keep embedded pages lightweight and avoid large external scripts.
- Test navigation and forms on mobile.
