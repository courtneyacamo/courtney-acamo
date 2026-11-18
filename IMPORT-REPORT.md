# Import report: Courtney Acamo

Imported from page.zip on 2026-11-18 with `openspace import html`.
Sources: the page's HTML and CSS. 1 requests.

## Summary

- **4** pages, **0** collection items in 0 collection(s)
- **19** media files (0.0 MB) downloaded into `media/`
- **0** redirects so old addresses keep working
- **10** item(s) need your attention (below)

## Pages

| Old address | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Remember the wellspring within | 3 | 6 |
| `/offerings` | `/offerings` | Ceremonies for the body, the spirit & the voice | 1 | 3 |
| `/about` | `/about` | Hello, I'm Courtney | 1 | 1 |
| `/book` | `/book` | Let's begin with a gentle hello | 1 | 1 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying the original site's CSS or code.

- Brand color #c9a04e (the site's accent color).
- Fonts on the original site: Cormorant Garamond / Jost → pairing "Cormorant Garamond & Jost" (Cormorant Garamond / Jost), same family for Cormorant Garamond and Jost. Licensed fonts can be uploaded in Site Styles → Fonts.
- Buttons on the original site have a gradient fill → the "pill-gradient" button style.
- The contrast solver adjusted 3 color pairing(s) so every section theme meets WCAG AA (e.g. light accent, light accent-hover).
- Page background #fbf8f1 on the original site → #fdfaf6 (text contrast 15.6:1).

Design check: 0 error(s), 20 warning(s).

- warning (/): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/offerings): Four sections in a row use the light color theme, so the page reads as one long block.
- warning (/about): This section's blocks are all empty.
- warning (/about): “Hello, I'm Courtney” has no clear call to action — nothing tells visitors what to do next.
- warning (site): The Hi, I'm Courtney section uses 4 fixed colours, so Site Styles can't restyle them.
- warning (site): The Ways we can gather section uses 8 fixed colours, so Site Styles can't restyle them.
- warning (site): The Invitation section uses 4 fixed colours, so Site Styles can't restyle them.
- warning (site): The How we'll walk together section uses 4 fixed colours, so Site Styles can't restyle them.
- warning (site): The Letters from the stillness section uses 8 fixed colours, so Site Styles can't restyle them.
- warning (site): The Ceremonies for the body, the spirit &… section uses 16 fixed colours, so Site Styles can't restyle them.
- warning (site): The Tea Ceremonies section uses 9 fixed colours, so Site Styles can't restyle them.
- warning (site): The Blessing Ceremonies section uses 13 fixed colours, so Site Styles can't restyle them.
- … and 8 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Forms and newsletter

- Newsletter signup recreated. The old site didn't keep a subscriber list itself: if its form sent sign-ups to an email service, export the list there and import it in the Hub. _(/)_
- Form "Contact form" recreated with 6 field(s). Submissions now arrive in the OpenSpace inbox; the original site form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/book)_

### Links

- Text link to /index.html led to a page that wasn't imported; the link was removed. _(/)_
- Text link to /offerings.html led to a page that wasn't imported; the link was removed. _(/)_
- Text link to /about.html led to a page that wasn't imported; the link was removed. _(/)_
- Text link to /book.html led to a page that wasn't imported; the link was removed. _(/)_
- Link to /offerings.html led to a page that wasn't imported; it now points at the home page. Point it at the right page. _(/)_
- Link to /book.html led to a page that wasn't imported; it now points at the home page. Point it at the right page. _(/, /offerings)_

## Not moved by the importer

- Scripts, animations and anything rendered only by JavaScript (try `--render` for script-built pages).
- Server-side features: shops, logins, search, comments.
- Form submissions, newsletter subscribers, member accounts and comments.
- Analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:migrate https://site.openspace.invalid` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (your registrar or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the old hosting until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain if you like).


## Designed sections

18 sections keep their own design as a designer component. Every word, picture and link in them is a field you edit in Studio; the design itself changes only through Component code (designers) or Claude.

| Section | Page | Fields | CSS |
|---|---|---|---|
| Hi, I'm Courtney (`hello`) | / | 6 | 2.2 KB |
| Ways we can gather (`offerings`) | / | 7 | 2.5 KB |
| Invitation (`invitation`) | / | 2 | 1.7 KB |
| How we'll walk together (`journey`) | / | 5 | 1.9 KB |
| Moments (`moments`) | / | 2 | 2.1 KB |
| Letters from the stillness (`letters`) | / | 2 | 2.1 KB |
| Ceremonies for the body, the spirit &… (`offerings-temple`) | /offerings | 14 | 3.1 KB |
| Tea Ceremonies (`offerings-tea`) | /offerings | 8 | 2.4 KB |
| Blessing Ceremonies (`offerings-blessing`) | /offerings | 9 | 2.9 KB |
| Intuitive Healing Sessions (`offerings-healing`) | /offerings | 8 | 2.4 KB |
| Not sure which is right for you? (`offerings-reach-out`) | /offerings | 4 | 1.6 KB |
| Hello, I'm Courtney (`about-temple`) | /about | 13 | 3.7 KB |
| Glimpses (`about-glimpses`) | /about | 1 | 2.1 KB |
| What I hold sacred (`about-sacred`) | /about | 7 | 2.3 KB |
| Sit with me (`about-sit-with-me`) | /about | 5 | 1.7 KB |
| Let's begin with a gentle hello (`book-temple`) | /book | 9 | 3.0 KB |
| Send a note (`book-book`) | /book | 9 | 3.4 KB |
| Footer (`site-footer`) | footer | 5 | 1.9 KB |

Sections that use OpenSpace's own section designs instead:

- /: CSS line 1: "--night-2" isn't a CSS property
- /offerings: CSS line 1: "--night-2" isn't a CSS property
