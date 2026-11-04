# Lady L Cannabis, redesigned ("Archway"): an unofficial preview

> **Unofficial.** This is an unofficial redesign preview of ladyljerseycity.com. It is not operated by,
> affiliated with or endorsed by Lady L Cannabis or its operator, Lady L Cannabis LLC. The live site is
> https://ladyljerseycity.com/.

**Preview: https://chris-sgen.github.io/ladyljerseycity/**

A redesign of the 112 pages of **ladyljerseycity.com**, made from the pages as the live site served
them (see *Snapshot*) and changed for a public address that is not the business's, as listed under *Changes for
this public copy*. It is a static site with no build step, no dependencies and no backend. Every page asks
search engines not to index it (`noindex`).

Two terms used below. The **handoff build** is the private build of this redesign that this copy was made
from, with its documentation and audit files; it is not published ("handoff" is the name its pipeline gives
its packaged output and says nothing about a recipient). This **preview** is that build with the changes
listed under *Changes for this public copy*.

## What works, and where its links lead

| Part | In this preview |
|---|---|
| **Forms** | **Disabled.** The 3 forms (on `/cannabis-guide/`, `/contact-us/` and `/`) send nothing, with or without JavaScript; the button of each is disabled. The pages carry no note about it. |
| **Online store** | Not copied. The store is the store vendor's application, served by the live host under `ladyljerseycity.com/stores/`. The 4,582 links to it on 114 pages (the header's "Order Now", the Shop menu, the category tiles, the delivery and pickup buttons) open the live store there, and 40 links in the text open pages of the shop's menu at `shop.ladyljerseycity.com` (brands, categories, products, the sale). Anything ordered there is ordered from the shop. |
| **Loyalty programme** | The footer's "Sign Up For Loyalty" (114 links, one on every page) opens the store's own sign-up at `ladyljerseycity.com/stores/enterprise/lady-l/signup`, as on the live site. 4 links on `/events/jersey-city-lgbtq-pride-festival/` and `/rewards/` open the shop's loyalty sign-up at `lab.alpineiq.com`, and 2 open its members' wallet there, as on the live site. |
| **Age question** | Asked on a first visit to any page, in the words of the live store's own pop-up ("Are you at least 21 years old or a valid medical patient?", Yes or No). A yes is kept in the visitor's browser for the session, or for 30 days with "Remember me for 30 days" ticked, under this copy's own name (`ladyljerseycity-age`): it reads no answer given on the live site. A no keeps the question up with the live footer's line "For adults 21+.". The live pop-up's line that continuing agrees to the store's terms is not carried. With scripts off the page shows and the question does not, as on the live store. |
| **Site search** | Works: it searches this copy's pages, on its own `/search/` page. |
| **Maps** | The 115 map frames are Google's keyless map embed: 58 where the live pages show a map (the shop's address, or the area a page is about), and one in the closing "Location & Hours" band of each page whose live version has none. The shop's address opens Google Maps; the home page's "Get Directions" button opens the online store, as on the live site. |
| **Reviews** | The 8 Google reviews of the home page, as the live strip shows them: each reviewer's name, stars and words, in a carousel. The reviewers' profile photos are not shown. "write a review" opens Google. |
| **Photo feed** | The 8 Instagram posts the live home page shows, each a link to its post on Instagram. |
| **Phone and e-mail** | The shop's own number and e-mail address (`hi@ladylretail.com`). The live site covers its e-mail addresses with Cloudflare's e-mail protection (a script writes them back in the visitor's browser); this copy writes the shop's address out. The addresses of two people at the shop that the live legal pages print are not written out: a link to the live page stands in their place (4 places on 3 pages). |

## What comes from the live site, and what does not

| Part | Source |
|---|---|
| **Words, addresses, hours, prices, reviews, links** | The live site's, as its pages printed them. The live stylesheet shows every heading and button in capitals, so its editors typed them in any case ("Our core valueS", "order NOW"); here every heading and button label is set in title case, each word in the site's own spelling of it. The emoji the live pages show as pictures of Google's emoji set are shown as emoji characters. |
| **Pictures** | The live pages' own: 114 pictures (each in one or more sizes), among them two stock photographs. See *Pictures*. |
| **Generated picture and film** | One picture made for this redesign with an image model (`fal-ai/nano-banana-pro` at fal.ai): a night sky with yellow sparkles in the colours of the shop's archway art. From it, a silent five-second film made with a video model (`fal-ai/kling-video/o3/pro/image-to-video` at fal.ai), the picture as its first and last frame, in which the sparkles twinkle; it plays on a loop with no controls, and the picture is its poster (all a visitor sees who asks for reduced motion or saves data). It stands at the opening of the 29 pages that have no picture at their opening on the live site (most of them events). It shows no product, place or person. |
| **Visual design** | New ("Archway"), drawn from the shop's own archway art (the arch, its coloured bands, the sparkles, the checkerboard), in the live site's colours, with a layer of glass over it: the cards, boxes and forms are frosted panes over a still field of the brand's colours, and the header, the menus and the opening of each page blur what passes under them. Every line of text was measured against what is drawn behind it, at four screen widths: none is under 4.5:1. |
| **Typefaces** | Bricolage Grotesque and Figtree, under the SIL Open Font License 1.1 (the licence texts are in `assets/fonts/`). |
| **Code** | Written for the redesign: three stylesheets (the site's, one for browsers without JavaScript, and this copy's notes) and one script. No WordPress, no page builder, no form plugin, no analytics or tracking script. |

## Pictures

- **People.** The live pages show photographs of people at events the shop held or joined (a garden party, a
  costume contest, a restaurant's birthday), in its Instagram feed (among them a raffle winner), in its own
  photographs (a model with the shop's tote bag) and in two stock photographs (Unsplash). This copy shows them where
  the live pages show them. The reviewers' profile photos of the review strip are not shown.
- **Pictures made by AI models.** 3 of the live site's own pictures are marked as made by AI models: 1 by a C2PA
  record of Google's that names it as made by a generative model, and 2 by the file names ChatGPT gives
  its images. Their files in this copy, and the files of the generated picture above, carry the IPTC label of a
  picture made by a generative model (`DigitalSourceType: trainedAlgorithmicMedia`, in an XMP packet): 26
  files. No other picture file carries any metadata but the colour profile its encoder writes.
- **The generated film.** Its 2 files (two sizes) carry no metadata at all: no tag, no provenance box, no creation
  time. This README and `PROVENANCE.md` are its label: it was made with an AI video model (see above).
- **A section the live site does not show.** The live home page's markup holds a section "Why Choose Us" that
  the live stylesheet hides at every screen width. It is not shown here either.

## Changes for this public copy

1. **`noindex, nofollow, noarchive, nosnippet, noimageindex` on every page.** This is the only control here that search engines honour, and it is a
   request. This copy's own `robots.txt` (it allows crawling, so that a crawler can read the noindex tag)
   and `sitemap.xml` are shipped, but crawlers read `robots.txt` only at the root of the host
   (`chris-sgen.github.io/robots.txt`), not under `/ladyljerseycity/`. GitHub Pages cannot send an
   `X-Robots-Tag` header, so the pictures and other files have no index control of their own;
   `noimageindex` asks search engines not to index the pictures a page shows. The repository itself is
   public, and its pages on github.com can be indexed.
2. **Link-preview tags:** `og:url` points at this preview; `og:description` and `twitter:description`
   carry the disclosure; `og:site_name` reads "Unofficial preview (not Lady L Cannabis)"; `og:title` and `twitter:title`
   begin "Unofficial preview:". The picture tags (738) are removed, and the shop's icons are not
   this copy's icon (342 icon links removed). What a link card shows depends on the app.
3. **Structured data removed** (226 JSON-LD blocks): it stated the business's identity, address,
   telephone and opening hours as data.
4. **Every form of the business is inert, with or without JavaScript.** A hidden, disabled submit button and a
   hidden, disabled text field stand first in each form (so that pressing Enter submits nothing); each button is
   a disabled `type="button"`; each form has `action=""`, `method="dialog"` and
   `onsubmit="return false"`, and the hooks the script would use are removed. The fields can be typed in;
   nothing typed leaves the browser.
5. **Links.** `<meta name="referrer" content="no-referrer">` on every page, and every frame carries
   `referrerpolicy="no-referrer"` itself. 378 links of the live pages carried marks
   that tell their target where the visit comes from (Google's search-session marks on the links of the shop's
   address to Google Maps among them, and campaign marks): they are taken off. 4 links on
   3 event pages went through e-mail click counters (3 through the shop's,
   1 through another sender's): they lead straight to the address the counter led to. The
   4,700 links to the live site carry `rel="nofollow noopener"`. Each page's canonical address
   (and the previous and next pages of the blog list) names the page on the live site.
6. **No on-page banner.** The disclosure is carried by the link-preview tags (2) and by this README. Notes stand
   on the pages only where a page needs one: a note on
   the live site's `/terms-of-service/`, `/privacy-policy/` and `/accessibility/` that their words are the live site's.
7. **Not shipped:** `.htaccess`, `llms.txt`, `robots.txt`, `sitemap.xml`, `vercel.json`, `_headers` and `_redirects` and the feed `/category/blog/feed/` of the handoff build (they name the
   business's real addresses or are read only by other hosts), and 38 files nothing in this copy
   names (picture sizes and icons that only the removed link-preview tags, structured data and icon links named,
   and the emoji pictures).
8. **The review strip's line under each review that its vendor verifies it** ("Trustindex verifies that the
   original source of the review is Google.", 8 reviews) is taken out: the copy does not use that vendor.
9. The not-found page is addressed under `/ladyljerseycity/`; the shop's icons are replaced by an empty one; the comments
   of the stylesheets and the script are taken out; the footer's copyright line is the live site's own, and its name
   links to the live site.

## Verification

The browser figures were measured at the public address, https://chris-sgen.github.io/ladyljerseycity/, on 2026-11-04 05:40 UTC (November 4 at 12:40 AM EST).

| Check | Result |
|---|---|
| Every sentence of the live pages looked for on its rebuilt page (handoff build) | 11,936 checked: 11,916 found, 20 left out with a recorded reason, 0 missing |
| Words of each live page found on the whole rebuilt page, the parts left out on purpose set aside (handoff build) | 99.94% mean over 112 pages (words counted, not their order), lowest 98.79%; no page with 12 or more live words missing in a row |
| Links and controls on phones and tablets (handoff build) | PASS: 460 page loads; 19,326 links and controls measured at 390 and 768 px against a 44 px target, and nothing reaching past the screen |
| The site search (handoff build) | PASS: 52 queries, 111 index entries |
| The pipeline's gate (handoff build) | 18 PASS, 11 FAIL, 0 UNPROVEN; the checks that are not green are explained below |
| This copy, read again from the shipped files | 494 files besides the three documents (114 of them pages): 0 findings. 11,460 local references, each to a file of this copy |
| Binary files read for metadata | 358 WebP (26 with the AI label above, the others with only the encoder's colour profile), 2 SVG (no script, no metadata; the one embedded PNG holds picture data only), 6 WOFF2 (no metadata block) |
| The 113 pages in a browser at 1440 and 390 px, and the not-found page at 1440 | 227 page loads, 3,062 pictures drawn, none broken; no request outside `/ladyljerseycity/` but the map frames' |
| Site search | The query "hoboken" was answered with 5 results, every one inside `/ladyljerseycity/` |
| Forms, with scripts on and off | 24 trials on the 3 forms. In the 18 with the form as shipped or with one safeguard alone, Enter was pressed in a field and the button clicked: nothing was sent. In the other 6 every safeguard was taken off and the form was seen to submit, as were 4 plain control forms, so the test can see a submission |
| The checker itself | `preview-selftest.mjs` planted 119 defects in a copy of this tree; all 130 reports they must give were given. 114 of the 148 rules that read the files were exercised by a plant |
| At the public address | 113 pages and 88 other files fetched at https://chris-sgen.github.io/ladyljerseycity/: 314 byte-identical to the verified files, 0 different, 0 not answered |

**Why the gate's checks that are not green are not green** (they concern the handoff build):

- **C03 Every crawled page fetched successfully** (FAIL). The one address the crawl could not fetch is Cloudflare's e-mail cover (`/cdn-cgi/l/email-protection`), not a page: the live site puts it in place of its e-mail addresses. The handoff build writes the addresses out (the shop's as an e-mail link, two others in running text as text); this copy writes out only the shop's (see *What works*).
- **C04 Content captured for every page** (FAIL). The 18 pages with almost no text are the online store's: the store vendor's application, which draws its pages in the browser. They are linked, not copied (see *What works*).
- **C05 No page is an unresolved JS-rendered shell** (FAIL). The same 18 store pages, drawn by scripts.
- **C07 Image inventory completed with real dimensions** (FAIL). Seven picture addresses have no file: icons of the store application, one picture named only by an unused stylesheet rule, and two backgrounds at another host (`ladyltest.deeproots.io`) whose name no longer resolves (the files of the same names in the site's own uploads are used).
- **C16 Every source page exists in the rebuild** (FAIL). The missing pages are exactly the 18 store addresses (linked, not copied).
- **C17 Content survived the rebuild** (FAIL). The live theme has no `<main>` element, so the gate compares each whole live page, menus and footer included, with the content of the rebuilt page. Compared whole page to whole page, with the parts left out on purpose named (the header that the live theme prints four times among them), mean recall is 99.94% over 112 pages; the one section reported lost ("Why Choose Us" on the home page) is hidden at every screen width by the live site's own stylesheet.
- **C18 SEO survived the rebuild** (FAIL). The losses are the store addresses; the "next page" link in the heads of `/events/` and `/service/` (the live host serves their page 2 as a copy of page 1, line for line; the redesign shows each whole list once); the alt texts of the review strip's icons and reviewers' photos and of the two pictures in the hidden section; and the main heading of 12 pages, set in title case where the live page typed it otherwise (the same letters; the live stylesheet shows every heading in capitals).
- **C20 No invented content** (FAIL). The flagged phrases are the live site's own: the titles of a post and of a page with the word "best", and the eight Google reviews, quoted word for word with the reviewers' names.
- **C21 No trace of the source platform** (FAIL). Six links to three documents on the websites of two other organisations, whose own addresses contain `/wp-content/`; the build itself names no part of the old platform.
- **C22 Design matches the source pixel-for-pixel at every breakpoint** (FAIL). This is a redesign: it is not meant to match the live site pixel for pixel.
- **C29 SEO emitted and derivable fields repaired** (FAIL). The checker decodes the sitemap's addresses but not the page addresses it compares them with, so the two pages whose addresses hold an emoji are reported missing from a sitemap that lists them.

## Snapshot

- Pages: read from https://ladyljerseycity.com between 2026-11-02 23:50 UTC (November 2 at 6:50 PM EST) and 2026-11-02 23:53 UTC (November 2 at 6:53 PM EST).
- Pictures: downloaded until 2026-11-03 00:25 UTC (November 2 at 7:25 PM EST); the photo feed's 8 pictures at 2026-11-03 01:26 UTC (November 2 at 8:26 PM EST).
- The live pages in a browser: 2026-11-03 00:26 UTC (November 2 at 7:26 PM EST) to 2026-11-03 01:33 UTC (November 2 at 8:33 PM EST).
- The second pages of two lists (`/events/page/2/`, `/service/page/2/`): fetched once on 2026-11-03 05:00 UTC (November 3 at 12:00 AM EST).

Hours, offers, events and reviews are as the live site showed them then.

## Rights

The words, pictures, names and marks of the live site belong to Lady L Cannabis LLC and to the others they
name; this copy claims no right in them. The typefaces are under the SIL Open Font License 1.1. `PROVENANCE.md`
and `PROVENANCE.json` say where everything came from and give the counts of the changes.
