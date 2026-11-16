# GreenScenez Landscape Management — GitHub Pages Website Concept

A polished, responsive, no-build, multipage website concept for **GreenScenez Landscape Management LLC** of Danielsville, Georgia.

## Contents

- `index.html` — home
- `about.html` — about the company
- `services.html` — service overview
- `contact.html` — quote/contact form
- `privacy.html` — draft privacy page
- `404.html` — custom not-found page
- `assets/` — CSS, JavaScript, brand marks, decorative SVG illustrations
- `docs/BRAND-GUIDE.md` — proposed identity and typography
- `docs/SOURCES-AND-NOTES.md` — research and editorial review notes

**Site is entirely static.** No npm, build step, Supabase, Netlify, or database required. All internal links and asset paths are relative, so it works in GitHub Pages project repositories such as `username.github.io/greenscenez/`.

## Deploy on GitHub Pages

1. Create a repository (for example `greenscenez-website`).
2. Upload the **contents of this folder** to the repository root, not the outer folder.
3. Commit changes to the `main` branch.
4. Go to **Settings → Pages → Build and deployment**.
5. Choose **Deploy from a branch**; select `main` and `/ (root)`. Save.
6. Visit the `github.io` URL GitHub displays once deployment completes. Test every page and the mobile navigation.

## IMPORTANT — Contact form activation

The HTML form uses https://formsubmit.co/ to deliver emails to `greenscenezgslm@gmail.com` using a normal POST. There is **no JavaScript-only simulation**.

1. The first submission normally triggers an activation email to the mailbox.
2. GreenScenez must open that email and activate the forwarding endpoint.
3. After approval, submit another test request and confirm arrival in the inbox.
4. The business should approve use of its address before publishing or accepting real visitor inquiries.

**Until activated and tested, do not represent the form as already verified.** The form has required-field validation and a spam honeypot. It will show FormSubmit's default confirmation page, not a site-specific local thank-you page. The `privacy.html` language is draft only.

## Photos

Per the project brief, **no AI-generated landscape photography is included**. Facebook photos were not available for confirmed retrieval and rights. The site uses original abstract/ornamental SVG graphics instead. When the business approves actual photos from its Facebook page, add optimized `.webp` files in `assets/` and replace the hero/feature art where desired; avoid embedding direct `facebook.com` CDN URLs, which can expire or block hotlinking.

## Brand and launch checklist

- [ ] Get GreenScenez's approval for brand concept, logo and page copy.
- [ ] Verify service availability, hours and coverage areas with the owner.
- [ ] Request and license authentic GreenScenez job-site photos and replace concept graphic panels where appropriate.
- [ ] Activate and test FormSubmit delivery, including mobile.
- [ ] Have business review privacy text and consent wording.
- [ ] Remove `<meta name="robots" content="noindex,nofollow">` from all HTML files **only when the site is approved for public indexing**.
- [ ] Add canonical URL, robots.txt, sitemap.xml and social image when the final custom domain is chosen.
- [ ] Configure the custom domain in GitHub Pages and your DNS provider if desired.

## Tech

- Lightweight HTML5/CSS3 + vanilla JavaScript.
- Accessible mobile navigation and FAQ, keyboard focus indicators, reduced motion support.
- Scroll reveals with IntersectionObserver, graceful fallback.
- LocalBusiness JSON-LD for phone/address/service area; no invented review markup.
- Responsive layout from 360px upward, uses relative links.

Designed as a pitch concept by Hutzell Creative Co. This is not yet the company's endorsed production website.
