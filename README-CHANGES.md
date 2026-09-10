# What changed, and what to double-check

## Before you upload
1. **Discord link** — I didn't have your real invite link, so `contact.html` has
   `href="#"` on "Add me on Discord." Search for `href="#"` and swap in your
   actual invite URL.
2. **Image filenames** — I rebuilt the pages using the filenames from your
   GitHub file listing (`project1.png` through `project12.png`, `Mimic.gif`,
   `me.jpg`, `meme.jpg`, `logo.png`), matched to captions in the same order
   they appeared on your old projects page. I could only see filenames, not
   the images themselves, so **open `projects.html` and check each
   `<img src="...">` actually points at the right screenshot** — swap any
   that are mismatched. `project1.png` wasn't used (I had one more filename
   than caption); feel free to slot it into whichever chamber card is wrong,
   or add a 13th project.
3. Drop `index.html`, `projects.html`, `contact.html`, `styles.css`, and
   `script.js` into your existing repo alongside your current images —
   nothing else needs to move.

## What I changed on top of the visual redesign
- Fixed a handful of typos in your bio ("Im" → "I'm", "comission" →
  "commission", "atpmosphere" → "atmosphere", "rouge AI" → "rogue AI") —
  your voice and wording are otherwise untouched.
- Turned the Languages/Software/Hardware lists into scannable tag chips.
- Added category tags + filter buttons (All / Rigging / Animation / Render /
  Scripting / Modeling) to the projects grid — I guessed each category from
  the title, so re-tag anything I got wrong via the `data-category`
  attribute on each `<article class="project-card">`.
- Made the whole site responsive (mobile hamburger nav, stacking layout) —
  the original didn't appear to have a mobile layout.
- Added a favicon, page titles, and meta descriptions per page.
- Respects `prefers-reduced-motion` and has visible keyboard focus states.

## Design concept
Leaned harder into the Aperture Science test-chamber voice you'd already
started (the aperture logo, "Communication Directives"): cut-corner console
panels instead of rounded cards, bracketed `[ SECTION ]` terminal labels,
a slow-spinning aperture mark, a "CAM_01" viewfinder frame around your
profile image, and the Wheatley meme restyled as "archive footage." Font
pairing is JetBrains Mono (terminal/display) + Manrope (body text).
