# Favorites Page

A clean, interactive favorites tracker built as a single standalone HTML file — no frameworks, no dependencies, no install needed.

## Live Demo

[abhijeetsinghdevgan.github.io/favorites-page](https://abhijeetsinghdevgan.github.io/favorites-page/)

## Overview

Bookstores, video games, podcasts, streaming services, and social platforms all have a favorites section. This page brings them all together in one place — letting you heart, save, and manage your favorites across five categories.

## Features

- **5 categories** — Bookstores, Video Games, Podcasts, Streaming Services, and Web Platforms
- **Heart toggle** — click the heart on any card to favorite or unfavorite it
- **Saved panel** — click the counter in the header to view all favorited items as removable chips
- **Persistent favorites** — saved to `localStorage` so they survive page refreshes
- **Toast notifications** — subtle confirmation on every save or remove action
- **Badges** — Top, Hot, and New labels on select cards
- **Responsive grid** — adapts to desktop, tablet, and mobile screens
- **Dark theme** — deep navy and gold palette, easy on the eyes

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript

## Getting Started

```bash
git clone https://github.com/abhijeetsinghdevgan/favorites-page.git
cd favorites-page
open index.html
```

No build step. No package manager. Just open the file.

## Customization

All content lives in the `DATA` object and `SOCIAL` array inside the `<script>` tag at the bottom of `index.html`.

Each item has the following shape:

```js
{ id, emoji, title, meta, sub, stat, statLabel, tag, badge }
```

To add a new category, add a new tab button in the `<nav>`, a new `<section>` in the markup, a new array in `DATA`, and call `renderGrid()` in the init block at the bottom.

The gold accent color is `#e8c97a` and the background is `#0f0f17` — both are defined as CSS custom properties in `:root` for easy theming.

## License

MIT — free to use for personal and commercial projects.
