# Lab Work #3 — Adaptive and Email-Compatible Layouts

**Course:** Web Application Development  
**Year of Study:** 2 | **Semester:** 1 | **Year:** 2024

**Author:** Maksym Poliukhovych

---

## Description

A tea-themed multi-page website implemented in three variants to demonstrate different layout approaches: a standard desktop layout, a mobile-adaptive version with media queries, and an email client-compatible version built with inline styles and table-based layout.

## Page Variants

| File | Purpose | Stylesheet |
|------|---------|------------|
| `index.html` | Standard desktop layout | `styles.css` |
| `index_mobile.html` | Mobile-adaptive (responsive) | `styles_mobile.css` |
| `index_postal.html` | Email client compatible | Inline styles only |

### Key differences

- **Desktop** (`index.html`) — CSS Grid layout, external stylesheet, full multi-column structure with left sidebar, main content, and right sidebar.
- **Mobile** (`index_mobile.html`) — CSS Grid layout with a `@media` breakpoint at `max-width: 720px` / `max-aspect-ratio: 9/16` that collapses the layout for small screens and portrait orientation.
- **Email** (`index_postal.html`) — No external CSS. All styles are inline. Uses `display: table` / `display: table-cell` for layout, ensuring compatibility with email clients that strip `<style>` blocks.

## Page Structure

All three variants share the same content:

- **Header** — site title and subtitle
- **Left sidebar** — fun facts about tea
- **Navigation** — links between all pages
- **Main content** — tea overview text, tea type descriptions, interactive image map
- **Right sidebar** — external articles and contact info
- **Footer** — author link

## Tea Pages

- `matcha.html` — Matcha
- `puer.html` — Puer
- `oolong.html` — Oolong
- `carcade.html` — Hibiscus (Karkade)

## Demo

[View on GitHub Pages](https://marshmalllows.github.io/web-lab3/)

## Technologies

- HTML5 (semantic markup, image maps, `<meta name="viewport">`)
- CSS3 (Grid, media queries, inline styles for email compatibility)
