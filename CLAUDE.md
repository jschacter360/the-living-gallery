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
- /assets — images, fonts, shared css/js

## Conventions
- Semantic HTML, mobile-first CSS.
- Image filenames: artist-slug_piece-slug.jpg
- Commit messages: short, present tense (e.g. "add spring show gallery")
- Ask before restructuring folders or deleting content — check with me first.
- Post layout default (see the first `.post` block in index.html): a
  `.post-meta` row with the date on the far left and the name/location on
  the far right, above a `.post-photos` grid using the largest ("_lightbox")
  version of each image, 2 per row, centered.