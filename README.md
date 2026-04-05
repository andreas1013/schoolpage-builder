# SchoolPage Builder

A self-contained HTML tool that helps Queensland schools create beautiful, SharePoint-safe content zone pages.

Schools fill in their content, click **Generate**, and get clean HTML to paste into a SharePoint Embed web part.

## Live Demo

Once deployed to GitHub Pages, the tool is accessible at:
`https://YOUR-USERNAME.github.io/schoolpage-builder/`

---

## Deploy to GitHub Pages (5 minutes)

1. **Create a new GitHub repository** (e.g. `schoolpage-builder`)
2. **Upload `index.html`** to the root of the repository
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`
5. Click **Save** — your site will be live in ~60 seconds

---

## How to use the tool

1. **Enter your Anthropic API key** in the banner at the top
   - Get one at [console.anthropic.com](https://console.anthropic.com/settings/keys)
   - The key is saved in your browser's local storage — you only need to enter it once
   - The key is never sent anywhere except directly to Anthropic's API

2. **Set your school name and brand colours** in the top bar

3. **Add content blocks** using the buttons at the bottom left:
   - **Banner** — coloured hero box with title and subtitle
   - **Image** — full-width photo (paste a SharePoint or public image URL)
   - **Info bar** — key details like Email and Opening Hours
   - **Text** — body paragraphs (blank line = new paragraph)
   - **Section** — heading in your primary colour + body text
   - **Sub-sections** — grouped content with headings, body text, and bullet links
   - **Tiles** — clickable 3-column grid (great for program listings)
   - **Callout** — highlighted info/warning/success box

4. **Click Generate** — Claude AI builds a styled, SharePoint-safe HTML fragment

5. **Click Copy HTML** — paste it into SharePoint:
   - Edit your page → **+ Add a web part** → search **Embed** → paste HTML → **Republish**

---

## Notes

- The generated HTML contains no JavaScript, no external fonts, and no CDN links — it is fully compatible with SharePoint's Embed web part restrictions
- All styles use system fonts (Arial, Helvetica, Georgia)
- The tool makes direct API calls to Anthropic from your browser — your API key is stored only in your browser's localStorage
- Generation takes approximately 10–20 seconds

---

## Content block reference

| Block | Use it for |
|-------|-----------|
| Banner | Page hero with title, subtitle, and school colour background |
| Image | Full-width photo below the banner |
| Info bar | Quick-reference details (email, phone, hours) |
| Text | Intro paragraphs or general body content |
| Section | A named section with a coloured heading |
| Sub-sections | A section with multiple named sub-topics, each with body text and bullet links |
| Tiles | Clickable program/activity cards in a 3-column grid |
| Callout | Highlighted info, warning, or success message |

