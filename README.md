# Whoop Whoop Technology — website package

Static site. No build step, no server-side code. Upload the contents of this folder to the web root of your host (e.g. public_html) so that index.html sits at the root.

## Files
- index.html — the whole site (HTML, CSS and JS in one file)
- film/ — the explainer video (how-ai-adoption-works.mp4, 102 s) and the Learning on Country clip, with poster images
- logo/ — favicon, app icon and primary logo PNGs
- (vector SVG/PDF logo files available on request)

## Before launch — placeholders still in the page
Search index.html for the square-bracket placeholders and replace them:
- [PHONE NUMBER]
- [EMAIL ADDRESS]
- [STREET ADDRESS]
- [ABN]
- [OUR ARTWORK] — the story of the commissioned artwork
- "Supply Nation (certification in progress)" in the hero eyebrow — change once certified, or remove if not yet applied for

## The enquiry form
The form currently shows a thank-you message on screen only. To receive enquiries, point it at a form service or your CRM. Simplest options: Formspree, Netlify Forms, or a HubSpot/Microsoft form embed. In index.html, find `id="enquiry"` and either set the form's action to your endpoint or replace the submit handler.

## Fonts
Archivo, Source Sans 3 and JetBrains Mono load from Google Fonts. If you need the site to work with no outside requests, self-host these three fonts and update the stylesheet link.

## Hosting notes
- Any static host works: cPanel/Apache, Nginx, Netlify, Vercel, Cloudflare Pages, S3 + CloudFront, GitHub Pages.
- Serve over HTTPS. Make sure .mp4 is served with Content-Type video/mp4 and that range requests are enabled (default on most hosts) so the video scrubs and loops properly.
- Suggested domain: whoopwhooptech.com.au (also register whoopwhooptechnology.com.au and whooptech.com.au and redirect them).
- For .com.au you need an ABN; register the domain in the company's name once the ABN exists.

## Dark mode
The site follows the visitor's system theme automatically.
