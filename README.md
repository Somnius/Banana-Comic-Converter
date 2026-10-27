# Banana Comic Converter

Turn comic and manga files (CBZ, ZIP or PDF) into pages that fill an e-ink screen. It can find each panel and fit it to the screen, or simply cut every page into overlapping parts. Output as XTCH (Xteink devices), EPUB or CBZ.

**Everything runs in your browser. Nothing is uploaded and nothing is installed.**

**Live site: https://seethroughme.github.io/Banana-Comic-Converter/**

Use it only with files you own or have the right to convert for personal use.

If it saves you time: [Buy me a coffee](https://ko-fi.com/curseofthebanana)

---

## Quick start

1. Open the [live site](https://seethroughme.github.io/Banana-Comic-Converter/) (or open `index.html` locally in any modern browser).
2. Drop CBZ, ZIP or PDF files on the **Files** box, or click it to browse. Folders work too.
3. Choose reading direction (right-to-left for manga) and your screen preset.
4. Under **Output**, tick the screen shapes (Portrait, Landscape, Mixed) and file types (XTCH, EPUB, CBZ). One file is made for every combination. XTCH is on by default.
5. Under **Panels**, pick **Smart panels** or **Simple page split** (see below).
6. Tick "I own these files", press **Convert**, then download. For batches, use "Download all as one ZIP". You can cancel at any time.

The small **i** next to each section explains it. **How to use** and **Tips and fixes** at the top open the full in-app guide.

## Two ways to convert

**Smart panels** detects panels, orders them for your reading direction, packs small panels together and enlarges long ones. A page-by-page editor lets you fix mistakes.

**Simple page split** skips all of that. Every page is cut into 2 (halves) or 3 (thirds) overlapping parts in reading order (overlap 8%, 15% or 25%), optionally after showing the whole page. Landscape screens get top-to-bottom bands; portrait screens show pages whole (wide spreads are cut left and right). Good for a quick conversion.

## Features

- **Input:** CBZ, ZIP (png, jpg, webp, gif, bmp) and PDF. Batch conversion, natural page sorting, cover first, credit pages last. Chapters from file or folder names, or PDF bookmarks.
- **Screens:** Portrait, Landscape, or **Mixed** (wide panels on landscape screens, tall panels on portrait screens, in one file). Device presets for Xteink X4 and X3, Kindle, Kobo and others, or a custom size.
- **Panel detection:** whitespace gutters with a fallback for busy pages, automatic detection of black gutters, reading order that handles tall panels beside stacked ones.
- **Zoom and splitting:** long panels are shown whole, then as two enlarged halves. Optional dense page zoom shows crowded screens whole, then as zoomed tiles. Cuts snap to blank gaps so speech bubbles stay whole where possible.
- **Packing:** small panels share a screen (max 1, 2 or 3) when they stay large enough.
- **Panel editor:** move, resize, draw, delete and reorder boxes; box shape lock to your screen's proportions; undo; a preview of the screens each box becomes; flags for pages that may need a manual look (several panels in one box, very big boxes) or a filter by panel count; keyboard shortcuts.
- **Image quality:** sharpen, e-ink contrast, darker midtones, screentone moire reduction, auto-levels, JPEG quality, and XTCH dither styles.
- **Metadata:** title, author, series, volume, publisher, year, language, description. Stored in EPUB and CBZ (ComicInfo.xml); XTCH keeps title, author, publisher and language.
- **Cover:** kept whole on a portrait page in landscape and mixed output.
- **Saved presets:** store all settings under a name (kept in your browser only).

## File types

| Type | Notes |
|------|-------|
| XTCH | 4-level gray container for Xteink devices. Landscape pages are stored sideways, so turn the device to read them. Options: rotation, dither style, experimental cover thumbnail. |
| EPUB | Fixed layout with a chapter table of contents and full metadata. |
| CBZ | Plain image pages plus a ComicInfo.xml. |

The XTCH output follows a community-written format description and has not been tested on every device. The cover thumbnail option is experimental. EPUB readers may not rotate automatically for mixed output.

## Your data

- Files are read and converted locally in your browser. Nothing is uploaded or shared.
- Presets and which sections are open are saved in your browser's local storage on that device only. Clearing site data removes them.
- Panel edits are kept only until you reload the page.
- The only outside link is the Ko-fi button.

## Hosting your own copy

The whole app is one file. Rename `banana-comic-converter.html` to `index.html` (all lowercase), put it in a public GitHub repository, then open **Settings > Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`. The site appears at `https://YOURNAME.github.io/REPONAME/` after a minute or two. Any static host works the same way.

## Credits and licences

- PDF reading uses [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla (Apache License 2.0), bundled in the page.
- Not affiliated with any device maker or publisher. Product and device names belong to their respective owners.
