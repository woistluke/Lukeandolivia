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

1. Drop your image files into the `images/` folder.
2. **Hero photo:** already set to `images/hero.jpg`. To swap it for a
   different photo, just replace that file with a new one of the same name
   (or edit the `url()` in the `.hero` rule in `css/style.css` to point at a
   different filename). Adjust `background-position` there if the photo
   gets cropped in a spot you don't like.
3. **Our Story photo:** already set to `images/story.jpg`. Swap it the same
   way as the hero photo — replace the file, or edit the `<img src>` in
   `index.html` inside `<div class="story-photo">`.
4. **Things To Do cards:** each `<div class="activity-photo">` can be swapped
   the same way — replace the emoji with an `<img>` tag.

## Colors & fonts

All colors and fonts are defined as variables at the top of `css/style.css`
under `:root`. Change a color once there and it updates everywhere. Current
theme is an editorial, photo-driven mountain look (cream/white background,
hairline dividers, a muted sage accent) with Cormorant Garamond for
headings/display type and Jost for body text — inspired by Zola's "Abbey"
template.

## Viewing your changes locally

Just open `index.html` in your browser — no server or install needed.

## Deploying

This is a static site, so it can be hosted for free on services like GitHub
Pages, Netlify, or Vercel, then pointed at your `lukeandolivialovebuttes.com`
domain via DNS.
