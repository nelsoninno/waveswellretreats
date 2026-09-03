# waveswellretreats.com

The website for Waveswell Retreats, Josselyn Alabi's stand up paddle surf
retreats in El Salvador. English at `/`, Spanish at `/es/`.

It is a plain static site. No WordPress, no database, no plugins, no monthly
software bill. Every page is a file you can open by double clicking it.

## Where things live

```
index.html              the English homepage
retreat.html            the retreat: price, dates, what is included, FAQ
coaching.html           one to one coaching and board rentals
about.html              Joss: story, competitive record, methodology
mar-de-suenos.html      the social project
guests.html             practical info for booked guests. Unlisted, not in Google
es/                     the Spanish version of every page above
assets/css/tokens.css   ALL the colours and fonts. Edit this to re-skin the site.
assets/css/styles.css   everything else about how it looks
assets/js/main.js       the mobile menu and the gentle fade-in
assets/images/          the photos used on the site, as .webp
llms.txt                what AI assistants read to describe the business
```

Your original photos, the brand sheet and the image manifest are kept in the
working copy of this project rather than in this repository, because everything
committed here is served publicly by the hosting.

## How to ask for a change

Send the change with enough detail that nobody has to guess:

- **A new photo:** send the original file, say which one it replaces, and give
  one sentence describing what is in it (that sentence becomes the alt text,
  which is what a blind visitor and Google both read).
- **New text:** send the exact wording you want, in English, in Spanish, or in
  Spanish and we will translate it.
- **A price or a date:** say what it is now and what it should become, and
  whether it changes in both languages.

Two rules keep the site working:

1. **Every change happens in both languages.** If a price changes on
   `index.html`, it changes on `es/index.html` too. A visitor reading Spanish
   should never see a different price.
2. **Colours and fonts only ever change in `assets/css/tokens.css`.** Never put
   a colour directly into a page.

## Where to drop new photos

Keep the original with the rest of your photos in the working copy. The web copy
goes in `assets/images/` under the right folder, saved as `.webp`, named like
this:

```
{what-it-is}-{who-or-what}-waveswellretreats.com.webp
```

For example `hero-joss-alabi-waveswellretreats.com.webp`. The image manifest in
the working copy lists every image slot on the site and what belongs in it.

## Things that must stay true

- No long dashes anywhere a person or a search engine sees them.
- Spanish keeps its real accents and its opening question and exclamation marks.
- Exactly one main heading per page.
- Every file stays under 25 MB. For video, use YouTube rather than uploading it.
- Links to files inside the site are relative (`assets/...`), never starting with
  a slash, so the pages still work when you open them from your own computer.

## Hosting

Cloudflare Pages, deployed from a GitHub repository. Pushing to the repository
publishes the site. There is nothing to log into day to day.
