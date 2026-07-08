# Project plan: Hobby Compass

## What this is
A single-page website, hosted on GitHub Pages, that asks the visitor a short
quiz about themselves and recommends a hobby based on their answers. A
compass needle animates to point at the result. There's also a "browse all
hobbies" section at the bottom of the page.

This is a first coding project. Priorities, in order:
1. Keep it working and simple over adding features.
2. Keep the code readable and commented — this is a learning project.
3. Every change should be small enough to test in the browser right after making it.

## Current state
- `index.html` — a complete, working first version. Single file: HTML, CSS,
  and JavaScript all together. No build step, no dependencies except two
  Google Fonts loaded via a `<link>` tag.
- Not yet in a GitHub repo or published.

## Tech constraints
- Must run as a **static site** — no backend, no database, no build tools
  (no npm, no React). Plain HTML/CSS/JS only, so it works directly on
  GitHub Pages.
- Keep it to as few files as reasonably possible while the project is small.
  It's fine to stay single-file until "Phase 3" below.
- No external JS libraries unless a phase specifically calls for one.

## Phase 1 — Get it live (do this first)
- [ ] Initialize a git repo in this project folder (if not already a repo).
- [ ] Create a GitHub repo (public) for this project.
- [ ] Push `index.html` to the `main` branch.
- [ ] Enable GitHub Pages in the repo settings, source = `main` branch, root folder.
- [ ] Confirm the live URL loads and the quiz works end to end (all 16
      questions, needle animates, restart button works, browse-all grid shows).
- [ ] Add a short `README.md` describing what the site is and linking to the live URL.

## Phase 2 — Polish the current version
Small, safe improvements to the existing single file. Do these one at a time,
testing in the browser after each:
- [ ] Add a favicon (a small icon shown in the browser tab).
- [ ] Improve mobile spacing — check the site on a narrow screen width (< 400px)
      and fix any cramped or overflowing sections.
- [ ] Add a subtle "your progress is saved" indicator — actually, skip local
      storage entirely (this is a personal-learning site, keep state in-memory
      only); instead just make sure refreshing the page always cleanly restarts
      the quiz.
- [ ] Double check color contrast is readable (light text on the dark
      background, dark text on the paper-colored hobby cards).
- [ ] Add a page `<meta name="description">` tag for search engines / link previews.

## Phase 3 — Split into multiple files (optional, once comfortable)
Only do this once Phase 1 and 2 feel solid — it's a good next learning step,
not a requirement:
- [ ] Split `index.html` into `index.html`, `styles.css`, and `script.js`.
- [ ] Update the `<link>` and `<script>` tags in `index.html` to point to the
      new files.
- [ ] Re-test the whole quiz still works after the split.

## Phase 4 — New features (pick and choose, not all required)
Ideas in rough order of difficulty:
- [ ] Add more hobbies to each category (currently 3 per category).
- [ ] Add more questions (currently 16).
- [ ] Show the visitor's top 2-3 categories as percentages after the quiz,
      not just the single winner (e.g. "60% active, 25% creative, 15% social").
- [ ] Let the visitor click any hobby in the "browse all" grid to see a longer
      description (a simple show/hide panel, no new page needed).
- [ ] Add a simple "share your result" button that copies a short text
      summary to the clipboard.
- [ ] Add a small animation or sound when the needle lands on the result
      (keep it subtle — this is optional polish, not required).

## Explicitly out of scope for now
- No user accounts or saved results across visits.
- No backend/server — everything must run as static files.
- No frameworks (React, Vue, etc.) unless a future phase is added specifically for learning one.

## How to work with Claude Code on this
- Tackle one checklist item at a time. After each change, open `index.html`
  in a browser and confirm nothing broke before moving to the next item.
- Ask Claude Code to explain any code it writes or changes, in plain terms,
  since the goal is learning — not just a finished site.
- Commit to git after each completed checklist item with a short message
  describing what changed.
