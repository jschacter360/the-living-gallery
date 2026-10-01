# A Little Lost

A static portfolio/blog site — a living gallery of my own photography and
work from other artists, such as visual art, fine art, music, cinema, design, and more, standing in for social media. Includes a shop
selling zines and photo prints to start, more products later.

## Stack
Plain HTML/CSS/JS, no build step, no framework. Deployed via GitHub Pages
from the `main` branch.

## Structure
- index.html — the gallery / landing page / main feed / chronological posts
- /POSTS — live on main feed in chronological order from newest to oldest 
- shop.html — zine and print listings
- archive.html — one-thumbnail-per-post archive of everything on index.html
- /assets — images, fonts, shared css/js

## Conventions
- Semantic HTML, mobile-first CSS.
- Image filenames: artist-slug_piece-slug.jpg
- Commit messages: short, present tense (e.g. "add spring show gallery")
- Ask before restructuring folders or deleting content — check with me first.
- Post layout default (see the first `.post` block in index.html): a
  `.post-meta` row with the date on the far left and the name/location on
  the far right, above a `.post-photos` grid using the "_bloginline" version
  of each image (sized for the feed's display width; "_lightbox" is reserved
  for a future full-size/zoom view), 2 per row, centered.
- Every `.post` article in index.html needs a unique, descriptive `id`
  (kebab-case, e.g. `id="post-paris-heat-waves"`) so archive.html can link
  straight to it.
- archive.html convention: when a new post is added to index.html, add one
  matching entry to the top of the `.archive-grid` (newest first, same order
  as the main feed). Each entry is an `.archive-item` link to
  `index.html#<that post's id>`, containing one `.archive-thumb` image (that
  post's "_thumbnail" file — the first/representative photo for a photo
  post, or the cover art's thumbnail for an audio post) and an
  `.archive-date` span with the post's date, shown at 8pt below the
  thumbnail.