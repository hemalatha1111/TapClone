<<<<<<< HEAD
# TapClone
=======
# 🖥 TAP Academy Website — Clone

> ⚠️ **Educational clone built for learning purposes only — not affiliated with TAP Academy.**
> Original site: https://thetapacademy.com

🔗 **Live Demo:** {{LIVE_URL}} · **Code:** {{REPO_URL}}

## 🎯 Goal
Recreate the TAP Academy homepage as pixel-close as possible in *layout and structure* — while
using an original color palette, type system, copy, and interaction design, to train my eye for
spacing, hierarchy, and responsive front-end craft rather than trace the original 1:1.

## ✅ Sections cloned
- [x] Navbar — logo, links, working login, mobile hamburger menu
- [x] Hero — headline, sub-text, CTA buttons, animated "terminal" signature element
- [x] Stats / placements strip — animated count-up numbers
- [x] Courses section (Java, Python, Data Science cards) with hover states
- [x] Why TAP Academy — 6-item feature grid
- [x] Testimonials — swipeable/autoplaying slider
- [x] CTA band + Footer with working `tel:` / `mailto:` links
- [x] Fully responsive (360px → desktop), tested at 360 / 390 / 768 / 1024 / 1440

## 🎨 Design decisions (why it isn't the same colors)
The brief asked for something *better than the original*, so this clone intentionally does not
reuse TAP Academy's orange/black palette. Instead:

- **Palette:** midnight-navy ink (`#0B1120`) base, amber (`#FFB020`) as the primary "achievement"
  accent, and mint (`#22D3B0`) as a secondary "code" accent — chosen to evoke a code-editor /
  terminal feeling appropriate for a coding bootcamp, rather than the source site's colors.
- **Type:** Space Grotesk (display/headings), Inter (body), JetBrains Mono (stats, tags, the
  hero's live-typing code snippet) — a three-role type system instead of one generic sans.
- **Signature element:** the hero features an animated terminal window that "types" a short code
  snippet and resolves into a placement badge — a visual metaphor for the site's core promise
  (code skills → job offer) instead of a generic hero graphic.

## ⚙️ Functionality notes
- **Login** is a fully working *front-end* flow (tabs for Log In / Sign Up, validation, loading
  state, toast confirmation, navbar swaps to a user chip with Log out). It is clearly labeled as
  demo-only in the modal since there is no backend/auth server behind this static clone.
- **Contact**: the phone number and email address are real `tel:`/`mailto:` links that work
  immediately, and the contact form hands off to `mailto:` with the message pre-filled — no
  backend is required for it to function.
- **Logo**: the official TAP Academy SVG could not be downloaded automatically (the CDN host
  wasn't reachable from the build sandbox). `assets/tap-academy-logo-white.svg` is an original
  wordmark I designed in the site's own type/color system as a stand-in — swap in the real
  asset from the link below if you have local network access:
  `https://d2hqh62t23qj3u.cloudfront.net/assets/TAP%20ACADEMY%20WHITE.svg`

## 📁 Structure
```
tap-academy-clone/
├── index.html      # all markup + CSS + JS (single-file, no build step)
├── assets/
│   └── tap-academy-logo-white.svg
└── README.md
```

## 🔍 Hardest part
Getting the hero's terminal typewriter and the testimonial slider to both feel intentional
(not like two unrelated widgets bolted onto a template) while still keeping every section usable
down to a 360px viewport — the terminal card in particular needed its own stacking/order rules
below 940px so it doesn't crowd out the headline on phones.

## 📸 Comparison
| Original | My clone |
|----------|----------|
| {{SCREENSHOT_ORIGINAL}} | {{SCREENSHOT_CLONE}} |

## ▶️ Running it
No build tools needed — open `index.html` directly in a browser, or serve the folder with any
static server (e.g. `npx serve .`).
>>>>>>> 17159a0 (Initial commit)
