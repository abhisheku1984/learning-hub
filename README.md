# The Learning Hub

Practical AI skills for work and career — a single-page site with tab-based page navigation by Abhishek Upadhyay.

**Live:** https://abhisheku1984.github.io/learning-hub/

## What's inside

- **One-page app with tab routing** — the top navigation stays fixed; each tab (Learn AI, AI Tools, Prompt Lab, Productivity, Career, Resume, Advertising, Projects, Achievements, About) opens its own page view via `#hash` routes. No scrolling between sections; browser back/forward and shareable URLs work.
- **Cinematic intro** — logo film → walking video, plays once per session on first open (skipped for `prefers-reduced-motion` users; Esc or the SKIP button exits).
- **Interactive tools** — searchable 20-tool library, 16 copy-paste prompts with clipboard copy, and an in-browser resume/ATS keyword checker (nothing is uploaded).
- **Free downloads** — `assets/downloads/` (prompt pack, tool guide, resume+ATS checklist).

## Structure

```
index.html              The entire app (markup, styles, logic, content data)
privacy.html            Privacy policy page
sitemap.xml / robots.txt
assets/
  logo-video.mp4        Intro logo film
  walking-video.mp4     Intro walking video (+ hero background)
  logo.jpg              Logo / favicon
  og-image.png          Social share card
  abhishek-*.jpg        Section imagery
  downloads/            Free resources
```

## Editing content

All content lives in the `const D = { ... }` object near the top of the large `<script>` in `index.html`:

| Key | What it controls |
|---|---|
| `learn` | Learn-page tracks and topics |
| `tools` | AI Tool Library cards |
| `prompts` | Prompt Lab cards |
| `prj` | Projects cards |
| `res` | Free Resources (name, category, level, description, file path) |
| `jr` / `aj` | Journey timeline and flow chips |

Videos/images referenced from `assets/` are set via the `VID`, `VID2`, `LOGO` constants at the top of the first script.

## TODO (owner)

- Add real LinkedIn / YouTube / Instagram URLs and a contact email (footer + follow buttons).
- Add real dates/roles to the journey timeline, plus certificates/awards when ready.
- Record and link real video lessons.
