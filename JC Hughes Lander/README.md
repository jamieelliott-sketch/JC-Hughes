# JC Hughes — Family Law Landing Page (GoHighLevel)

Pixel-perfect recreation of the mock lander, split into 5 standalone sections
for GoHighLevel. Brand colours: logo green `#35504c` (primary / backgrounds),
sage `#7dafa8` (sub-text, icons, accents — from the "Background colour" file),
cream `#f4f0ec` (light sections), white text.

## Files

| File | Section |
|---|---|
| `section-1-hero.html` | Hero: headline, bullets, call CTA + call-back form |
| `section-2-team.html` | Meet the team (6 headshots) |
| `section-3-how-we-help.html` | How will a lawyer help me? (01–04 grid) |
| `section-4-testimonials.html` | What our clients say (2 Google reviews) |
| `section-5-footer.html` | Footer: 3 offices + logo & badge |
| `preview.html` | All 5 stitched together — open in a browser to see the full page |
| `assets/` | Images to upload to GHL |

## How to install in GoHighLevel

1. **Upload images**: Media Library → upload the hero photo and the 6 team
   headshots from `assets/`. The logo loads from jchughes.net and the gold
   Accredited Specialist badge is embedded directly in the code (base64), so
   neither needs uploading — the badge always shows next to the logo.
2. **Build the page**: add one full-width section per file, each containing a
   single **Custom Code / HTML** element. Paste the whole file (styles included).
   Set section + row padding to 0 and page width to full/100% so the diagonals
   run edge to edge.
3. **Swap image paths**: in each pasted block, replace `assets/...` paths with
   your GHL Media Library URLs. They are:
   - Section 1: `assets/hero-bg.jpg`
   - Section 2: the 6 team headshots (named per person)
   - Sections 1 & 5: nothing else — badge and logo are already handled
4. **Wire the form**: the call-back form is styled HTML only — it will not
   create a GHL contact by itself. Either swap the `<form>` block for a GHL
   form embed (restyle to match), or keep the markup and attach your own
   submission script/webhook. Field names used: `full_name`, `email`, `phone`.
5. **Phone numbers**: the "Call now" pill and "free consultation" link dial the
   firm's freephone **0800 279 3090** (main number on jchughes.net). Footer
   office numbers are clickable tel links too. Change in the `tel:` hrefs if
   the client wants calls routed elsewhere (e.g. a GHL tracking number —
   recommended for Meta ads attribution).

## Copy changes vs the mock (the mock had placeholder text)

- Card 02 said "…may qualify for a **personal injury** claim" → reworded for family law.
- Card 03 said "With over … years" → "With over 35 years" (firm est. 1986).
- Form disclaimer was Canva's placeholder ("Your Canva profile name will be
  shared…") → "Your details are 100% confidential and will never be shared."

Everything else (layout, colours, diagonal section cuts, testimonials, footer
offices) follows the mock and the Footer file. Fully responsive — mobile stacks
the hero above the form and reorders the 01–04 grid correctly.
