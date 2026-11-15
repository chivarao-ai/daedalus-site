# Daedalus Automations website

Static site for daedalusautomations.com, served by GitHub Pages from the `main` branch.

## Files

- `index.html`: the whole site (text, styles and the language switch).
- `media/`: the two demo videos and their preview images.

## Updating the site in VS Code

1. Clone once: in VS Code run "Git: Clone" and paste `https://github.com/chivarao-ai/daedalus-site`.
2. Before each edit, open the Source Control panel and click Sync (or run "Git: Pull") to get the latest version.
3. Edit `index.html` and save. To preview, open the file in a browser.
4. In Source Control, write a short message, click Commit, then Sync.
5. The live site updates a minute or two later.

## Common edits

- **Text:** every visible sentence appears twice, once in `<span class="en">` (English) and once in `<span class="nl">` (Dutch). Change both.
- **Prices:** search for `class="price"` in `index.html`. The launch offer price is in the `#contact` section.
- **Contact details:** search for `class="mail"` and change the email address in both the link (`href="mailto:..."`) and the visible text.
- **Videos:** replace the files in `media/` and keep the same file names, or update the `src` and `poster` paths in the `#demos` section.
- **Colours and fonts:** the `:root` block at the top of the `<style>` section holds the colour and font tokens for light and dark themes.

## Domain

The custom domain is set in the repository's Settings > Pages. GitHub stores it in a `CNAME` file in this folder; do not delete that file.
