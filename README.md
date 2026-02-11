# MerrillLines — Personal Site

Personal portfolio site for Merrill Lines at [linesmerrill.com](https://linesmerrill.com).

## Tech Stack

- **Pure HTML/CSS/JS** — no build tools, no frameworks, no dependencies
- **Google Fonts** — [Syne](https://fonts.google.com/specimen/Syne) (display headings) + [Outfit](https://fonts.google.com/specimen/Outfit) (body text)
- **Formspree** — contact form backend (sends to linesmerrill@gmail.com)

## Design

- **Theme:** Dark glassmorphism with animated gradient mesh background
- **Colors:** Electric cyan (`#00e5ff`), hot magenta (`#ff2d78`), lime (`#b8ff57`) on deep dark (`#0a0a0f`)
- **Glass effect:** `backdrop-filter: blur()` with semi-transparent borders
- **Animations:** CSS keyframe blob floats, staggered fade-up entrance on hero, IntersectionObserver scroll reveals
- **Responsive:** Mobile hamburger nav, stacked layouts under 900px/640px breakpoints

## Deployment

Deployed via **GitHub Pages** from the `gh-pages` branch. Pushing to `gh-pages` triggers an automatic deploy.

### Custom Domain Setup (Squarespace DNS)

The domain `linesmerrill.com` is registered on Squarespace. DNS records needed:

| Host | Type | Data |
|------|------|------|
| `@` | A | `185.199.108.153` |
| `@` | A | `185.199.109.153` |
| `@` | A | `185.199.110.153` |
| `@` | A | `185.199.111.153` |
| `www` | CNAME | `Linesmerrill.github.io` |

The `CNAME` file in the repo root tells GitHub Pages to serve on the custom domain. In GitHub repo **Settings > Pages**, set custom domain to `linesmerrill.com` and enable HTTPS.

## File Structure

```
index.html    — entire site (HTML + embedded CSS + JS)
CNAME         — custom domain for GitHub Pages
img/avatar.jpg — profile photo
```
