https://cv.herremil.com/

## Notes

**`og:image:alt` is painted into `img/og-card.jpg`.** The tag transcribes the card
art verbatim, down to the `cv.herremil.com` line at the bottom left. Editing the
tag without re-rendering the JPG silently ships a card whose picture and alt text
disagree; nothing greps for it.

**Hosts.** `herremil.com/cv/*` 301s to `cv.herremil.com` with the path stripped,
so canonical, `og:url`, the `ProfilePage` node and `sitemap.xml` all use the `cv.`
host. The JSON-LD `Person` node intentionally stays on the `herremil.com` apex —
it is the same person across both sites, not a page on this one.
