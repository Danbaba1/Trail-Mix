# Trailmix landing page

A responsive landing page for **Trailmix**, a made-up weekend hiking club. It was built from a Figma design as the project for the *Design to code* module of the Lumen frontend course.

The goal of the project is to read a design's measurements and turn them into HTML and CSS that match it, on both desktop and mobile.

## Preview

Open `index.html` in a browser. There is no build step and no dependencies to install.

## Tech

- HTML5, with semantic elements (`header`, `main`, `section`, `article`, `footer`)
- Plain CSS: Flexbox, Grid, custom properties, media queries
- No JavaScript
- Fonts from Google Fonts: **Bricolage Grotesque** (headings) and **DM Sans** (body)

## Project structure

```
.
├── index.html   # page markup
├── styles.css   # all styles, including the mobile media query
└── README.md
```

## Page sections

| Section | Selector | What it contains |
| --- | --- | --- |
| Header | `.header` | Logo, navigation links, "Join the club" button |
| Hero | `#hero` | Badge, headline, intro, two buttons, illustration |
| How it works | `#how` | Three numbered steps in a grid |
| Hikes | `#hikes` | Three hike cards with illustrated images |
| Pricing | `#pricing` | Walker (free) and Member plans |
| Join | `#join` | Call-to-action card |
| Footer | `#footer` | Copyright and links |

## Design tokens

The colours from the Figma variables are defined as CSS custom properties on `:root`:

| Token | Value | Used for |
| --- | --- | --- |
| `--pine` | `#183D2F` | Headings, dark backgrounds |
| `--pine-2` | `#20493A` | Dark pricing card |
| `--moss` | `#2F6B4F` | Primary buttons, hero image |
| `--sun` | `#F2B544` | Sun, step numbers, join card |
| `--sand` / `--sand-text` | `#FCEFD0` / `#7A5410` | Badges |
| `--paper` | `#F6F4EE` | Page background |
| `--white` | `#FFFFFF` | Cards, header |
| `--stone` | `#5B6660` | Secondary text |
| `--ink` | `#3E4A44` | Body text |
| `--on-dark` | `#D7E2DB` | Text on dark backgrounds |
| `--line` | `#C3CDC5` | Secondary button border |
| `--mist` | `#DDE3DC` | Card and section borders |
| `--sky` | `#3D7A8C` | Hike card 2 background |
| `--forest` | `#7A8C3D` | Hike card 3 background |

## Responsive behaviour

The design has two Figma frames: **Desktop (1280)** and **Mobile (390)**.

- Above 950px, the layout is the desktop design: a two-column hero, a three-column steps grid, and hike and pricing cards in a row.
- At 950px and below, a media query switches to the mobile design: the sections stack in one column, the buttons fill the width, and the header shows a menu button instead of the links.

The hero illustration scales with its container. The sun is positioned from the right edge, and the mountain SVGs are anchored to the bottom at `width: 100%`.

## Known limitations

- The mobile menu button is a visual placeholder and doesn't open anything yet.
- The links in the header and footer point to in-page anchors or placeholder targets.
- The card illustrations in the hikes section use fixed-size SVGs, so they may clip slightly at some widths.

## Ideas for next steps

- Make the mobile menu work with a small amount of JavaScript.
- Make the hike card illustrations scale like the hero illustration.
- Add visible focus styles for keyboard users.
- Add a tablet layout between 600px and 950px.

## Credits

A practice design for Lumen's *Design to code* module. Trailmix is a fictional brand.
