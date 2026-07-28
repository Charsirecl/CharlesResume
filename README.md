# Charles Resume

Interactive, single-page personal site for Junxian (Charles) Li — software engineer
focused on full-stack, backend, and AI infrastructure work, with a tennis-themed
personal touch.

## Features

- Light/dark theme toggle (persisted, respects OS preference on first visit)
- Typewriter-style rotating role header
- Tabbed work experience, expandable project cards, and a flagship architecture
  diagram for the MCP / AI Data Gateway project
- "Beyond the Keyboard" section plus a hidden tennis rally mini-game (the
  floating **Rally** button, bottom-left)
- Contact form with a `mailto:` fallback until a live form endpoint is configured

## Local preview

Open `index.html` in a browser — no build step required.

## Configuration

Open `index.html` and search for the `Config` block near the top of the
`<script>` tag:

```js
var FORMSPREE_ENDPOINT = "REPLACE_WITH_YOUR_FORMSPREE_ENDPOINT";
var LINKEDIN_URL = "";
```

- **Contact form**: create a free form at [Formspree](https://formspree.io/) (or
  a similar service), then paste the endpoint URL
  (`https://formspree.io/f/xxxxxxx`) in as `FORMSPREE_ENDPOINT`. Until this is
  set, the form falls back to opening a pre-filled `mailto:` link.
- **LinkedIn**: paste your profile URL into `LINKEDIN_URL` to activate the
  LinkedIn icon and contact-section link.

## Publish with GitHub Pages

Push this repository to GitHub and enable Pages from the `main` branch root.
