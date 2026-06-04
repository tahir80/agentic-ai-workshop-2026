# Agentic AI for Life Sciences — Workshop Website

A static two-page website for the 4TU.NIRICT / WUR Agentic AI Workshop (1 July 2026).

## Files

```
workshop-site/
├── index.html       ← Main page: objectives, agenda, speakers
└── breakouts.html   ← Breakout sessions: LDJ method, groups, tools
```

## How to publish on GitHub Pages

1. Create a new repository on GitHub (e.g. `agentic-ai-workshop-2026`)
2. Upload both HTML files to the repository root
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` branch and `/ (root)` folder
6. Click **Save**

Your site will be live at:
`https://YOUR-USERNAME.github.io/agentic-ai-workshop-2026/`

## Adding speaker photos

To add real photos, replace the speaker initials placeholders in `index.html`.
Find each `<div class="speaker-img-wrap">` block and replace the inner content:

```html
<!-- Before (placeholder) -->
<div class="speaker-img-wrap">
  <span class="speaker-avatar-placeholder">BT</span>
</div>

<!-- After (with photo) -->
<div class="speaker-img-wrap">
  <img src="images/bedir-tekinerdogan.jpg" alt="Bedir Tekinerdogan" />
</div>
```

Then create an `images/` folder in the repo and upload the photos there.
Recommended: square images, at least 400×400px.

## Updating the registration link

In `index.html`, find the two registration links and replace `#` with your actual form URL:

```html
<a href="YOUR-REGISTRATION-LINK">Register Here →</a>
```

## Customising colours

All colours are defined as CSS variables at the top of each HTML file.
The main palette uses deep moss green (`#2d5a3d`) and warm gold (`#c8972a`).
