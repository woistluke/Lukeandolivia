# Luke & Olivia — Crested Butte Celebration Weekend

A simple, hand-editable website for our celebration weekend in Crested Butte.
No build tools, no frameworks — just plain HTML/CSS/JS so it's easy to edit yourself.

## Files

- `index.html` — all the page content, section by section
- `css/style.css` — all the styling (colors, fonts, layout)
- `js/script.js` — small bits of interactivity (mobile menu, FAQ accordion)
- `images/` — put your photos here

## How to edit content

Open `index.html` in any text editor. Every spot that needs your input is
marked with an `<!-- EDIT ME -->` comment right above it — things like:

- The weekend dates (hero section, schedule, footer)
- Your story (Our Story section)
- Schedule details (The Weekend section)
- Travel/lodging info (Travel & Stay section)
- RSVP link (RSVP section — replace `href="#"` with your Google Form/Zola link)
- Registry link (Registry section)

Search the file for `EDIT ME` to find every spot at once.

## How to add photos

1. Drop your image files into the `images/` folder (e.g. `images/hero.jpg`, `images/us.jpg`).
2. **Hero background photo:** in `css/style.css`, find the `.hero` rule and
   the comment above `.hero::before`, and follow the instructions there to
   swap the illustrated mountains for a real photo.
3. **Our Story photo:** in `index.html`, find `<div class="story-photo">`
   and replace its contents with `<img src="images/us.jpg" alt="Luke and Olivia">`.
4. **Things To Do cards:** each `<div class="activity-photo">` can be swapped
   the same way — replace the emoji with an `<img>` tag.

## Colors & fonts

All colors and fonts are defined as variables at the top of `css/style.css`
under `:root`. Change a color once there and it updates everywhere. Current
theme is a rustic mountain palette (forest green, bark brown, cream, rust
accent) with Fraunces for headings and Karla for body text.

## Viewing your changes locally

Just open `index.html` in your browser — no server or install needed.

## Deploying

This is a static site, so it can be hosted for free on services like GitHub
Pages, Netlify, or Vercel, then pointed at your `lukeandolivialovebuttes.com`
domain via DNS.
