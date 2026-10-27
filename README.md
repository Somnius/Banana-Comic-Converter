# Banana Comic Converter

Turn comic and manga files (CBZ, ZIP or PDF) into pages that fill an e-ink screen. It can find each panel and fit it to the screen, or simply cut every page into overlapping parts. Output as XTCH (Xteink devices), EPUB or CBZ.

**Everything runs in your browser. Nothing is uploaded and nothing is installed. No AI is used anywhere in the conversion: panels are found with plain image analysis (whitespace and border detection) that runs on your device, with no AI model and no online service.**

**Live site: https://seethroughme.github.io/Banana-Comic-Converter/**

Use it only with files you own or have the right to convert for personal use.

If you are happy with the results and enjoy your mangas/comics on your device, you can always [buy me a coffee (:](https://ko-fi.com/curseofthebanana)

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
- **Panel detection:** whitespace gutters with a fallback for busy pages, automatic detection of black gutters, reading order that handles tall panels beside stacked ones, and separation of panels that bleed into each other.
- **Batch edits:** convert, review, edit Metadata and panels for your files in batch and download them all as a zip folder.
- **Zoom and splitting:** long panels are shown whole, then as two enlarged halves. Optional dense page zoom shows crowded screens whole, then as zoomed tiles. Cuts snap to blank gaps so speech bubbles stay whole where possible.
- **Packing:** small panels share a screen (max 1, 2 or 3) when they stay large enough.
- **Panel editor:** move, resize, draw, delete and reorder boxes; box shape lock to your screen's proportions; undo; a preview of the screens each box becomes. All controls sit in one side column next to the page, with a progress bar for flagged, reviewed and remaining pages.
- **Zoom per box:** pick Auto, Off, overlapping Halves or overlapping Thirds for any single box.
- **Pages to check:** flags pages with several panels in one box, very big boxes or overlapping boxes (tall and busy boxes optional), or filters pages by panel count. Step through flagged pages only.
- **Keyboard shortcuts:** arrows change page, up/down or 1-9 pick a box, H / T / O / A set zoom, plus D, W, R, S, F, [ ], Delete and Ctrl+Z. The keys are shown on the buttons.
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
- No AI or machine learning is used during conversion. Detection is ordinary image analysis, so results are repeatable and you can correct any page in the editor.
- Presets and which sections are open are saved in your browser's local storage on that device only. Clearing site data removes them.
- Panel edits are kept only until you reload the page.
- The only outside link is the Ko-fi button.

## Credits and licences

- PDF reading uses [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla (Apache License 2.0), bundled in the page.
- Not affiliated with any device maker or publisher. Product and device names belong to their respective owners.
