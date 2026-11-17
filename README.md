# EIDORA documentation

A small, static user guide for the EIDORA graphical interface. Open `index.html`
in a browser to view it. No installation, build step, or JavaScript is needed.
The same files can be served by any static website host.

## Files

- `index.html`: introduction and links to the guide.
- `installation.html` and `quick-start.html`: getting started.
- `assets.html`, `metadata.html`, `embeddings.html`, `discovery.html`, and
  `figures.html`: the five workspaces.
- `troubleshooting.html`: help with common problems.
- `styles.css`: shared layout, colors, typography, mobile, and print styles.
- `assets/brand/`: the official EIDORA icon and wordmark, copied from
  https://www.eidora.org/assets/brand/ on 17 November 2026.

## Edit a page

1. Open its HTML file in a text editor.
2. Find the `Main documentation content` comment.
3. Replace the paragraphs marked `Placeholder:` with documentation. Remove
   `class="placeholder"` from finished paragraphs and remove the draft notice
   when the whole page is ready.
4. Save and refresh the page in a browser.

Keep one `<h1>` for the page title. Use `<h2>` for sections and `<h3>` for
subsections. Use `<ol>` for steps and `<ul>` for unordered lists. Write steps
using the exact labels visible in EIDORA. The initial section headings are an
outline, not verified instructions for a particular release.

## Add a page

Copy a similar HTML file and give it a descriptive, lowercase filename. Change
its `<title>`, description, heading, and article content. Update its section IDs
and the matching links under “On this page”.

Navigation is deliberately written directly in each file. Add the new link to
the sidebar in **every HTML page**, and place `aria-current="page"` only on the
link for that file. Update the previous/next links where appropriate. Shared
header or footer changes must also be made in every file.

## Keep it accessible

- Keep the skip link, `main` ID, navigation labels, and visible focus styles.
- Use descriptive link text and meaningful alternative text for screenshots.
- Put screenshots in `assets/images/` and use relative paths in `<img>` tags.
  Include a caption explaining what readers should notice.
- Check links with the keyboard and check the layout on a narrow screen and
  at enlarged text sizes. The sidebar moves above the article on small screens.
- Keep text readable against its background. Shared brand colors are listed at
  the top of `styles.css`; the site intentionally uses light mode only.

All content and assets are local. There are no analytics, external fonts, or
third-party scripts.
