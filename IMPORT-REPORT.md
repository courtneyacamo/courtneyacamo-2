# Import report: Courtney Acamo

Imported from https://www.courtneyacamo.com (Wix, Wix.com Website Builder) on 2026-11-17 with `openspace import url`.
Sources: page HTML, the sitemap. 110 requests.

## Summary

- **12** pages, **0** collection items in 0 collection(s)
- **92** media files (134.5 MB) downloaded into `media/`
- **0** redirects so old addresses keep working
- **8** item(s) need your attention (below)

## Pages

| Old address | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Home | 5 | 24 |
| `/intuitive-healing-sessions` | `/intuitive-healing-sessions` | Intuitive Healing Sessions | 5 | 16 |
| `/vocal-alchemy-sessions` | `/vocal-alchemy-sessions` | Vocal Alchemy Sessions | 8 | 19 |
| `/custom-immersions` | `/custom-immersions` | Custom Immersions | 16 | 54 |
| `/contact-me` | `/contact-me` | Contact me | 3 | 5 |
| `/bloom-retreat-may-2024` | `/bloom-retreat-may-2024` | Bloom | 15 | 33 |
| `/copy-of-home` | `/copy-of-home` | AWAKEN THE CURRENTS OF CREATION | 9 | 29 |
| `/copy-of-bloom-retreat-may-2024` | `/copy-of-bloom-retreat-may-2024` | Bloom | 15 | 32 |
| `/coming-soon-02` | `/coming-soon-02` | Medicine of the voice song circle | 1 | 2 |
| `/challenges` | `/challenges` | Sound Medicine Course | 2 | 1 |
| `/terms-and-conditions` | `/terms-and-conditions` | TERMS OF USE | 2 | 4 |
| `/pricing-plans/list` | `/pricing-plans/list` | Plans & Pricing | 1 | 1 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying Wix's CSS or code.

- Brand color #9f2747 (the site's accent color).
- Fonts on Wix: forum / avenir-lt-w01_35-light1475496 → pairing "Bricolage Grotesque & Geist" (Bricolage Grotesque / Geist), the closest curated match. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on Wix: Heading 1 is 4.0× body text. Density "comfortable" from the section heights.
- forum (a licensed font) can't be copied, so Forum — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- avenir-lt-w01_35-light1475496 (a licensed font) can't be copied, so Jost — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Type scale on Wix (the live site, measured in a browser) kept: display 130px/130px, heading 1 80px/80px caps, heading 2 80px/80px, body 20px/20px.

Design check: 1 error(s), 128 warning(s).

- **error** (footer): The section background (#826d45) leaves body text at 4.45:1 contrast; it needs 4.5:1.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this gallery block has no alt text, so people using screen readers won't know what it shows.
- … and 117 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Custom code and embeds

- Site-wide scripts were found (1: browser.sentry-cdn.com). They were **not** copied: add what you still need (analytics, chat) in Settings → Advanced. Wix-specific scripts won't work here. _(site)_

### Forms and newsletter

- Form "comp lpr9ocik1" recreated with 4 field(s). Submissions now arrive in the OpenSpace inbox; Wix form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/contact-me)_
- Newsletter signup recreated. Subscribers are not moved: export your list from Wix (or your email service) and import it in the Hub. _(/coming-soon-02)_
- Form "comp lrkkm5e8" recreated with 3 field(s). Submissions now arrive in the OpenSpace inbox; Wix form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(footer)_

### Links

- Text link to /intuitive-healing-session led to a page that wasn't imported; the link was removed. _(/, /copy-of-home)_
- Text link to /liberate-immersion led to a page that wasn't imported; the link was removed. _(/, /copy-of-home)_

### Design

- Layout: "AWAKEN THE CURRENTS OF CREATION": its background #ffffff, as on the original. _(/)_
- Layout: "AWAKEN THE CURRENTS OF CREATION": the image takes 8/12 of the width, as on the original. _(/)_
- Layout: "Lets work": the image takes 8/12 of the width, as on the original. _(/)_
- A photo section's overlay was darkened from 25% to 60% so its text stays readable. _(/, /vocal-alchemy-sessions, /custom-immersions, /bloom-retreat-may-2024, +3 more)_
- A photo section's overlay was darkened from 25% to 45% so its text stays readable. _(/intuitive-healing-sessions, /vocal-alchemy-sessions, /bloom-retreat-may-2024)_

### Other

- Wix strips and absolute-positioned layouts were turned into OpenSpace sections and columns; check spacing and alignment in the visual parity pass. _(site)_

## Not moved by the importer

- Wix apps: Stores, Bookings, Events, Members, Forum, Pricing Plans and Velo code (pages that show them are imported as content).
- Animations, scroll effects and strips' video backgrounds.
- Form submissions, newsletter subscribers, member accounts and comments.
- Analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:migrate https://www.courtneyacamo.com` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (Wix Domains, your registrar or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the Wix plan until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain if you like).

## Phones

Made 1 phone-only adjustment so the site reads well on phones (use a 40px logo on phones). The desktop design is unchanged.
