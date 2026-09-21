# Book 004 — FINAL pre-publish package (OWNER QA)

**DO NOT upload to KDP / Amazon until owner explicitly approves.**

## Title
Little One's Little Builder Construction Coloring Book  
(NO colon in title)

## Specs
| Field | Value |
|-------|-------|
| Trim | 8.5 × 11 in |
| Interior | B&W, 64 pages |
| Planned price | **$9.99** |
| Expanded Distribution | **OFF** |
| Imprint | Dairian's Bookstore |
| Copyright | 2026 |
| Paper (spine calc) | White — spine_in = 64 × 0.002252 = **0.144128 in** |

## Page map
| Pages | Content |
|-------|---------|
| 1 | Title art |
| 2 | Thank-you / belongs-to / copyright / AI disclosure |
| 3–58 | Coloring pages (56) |
| 59–63 | Blank / white |
| 64 | Colophon |

### Art provenance notes
- **Pages 3–26:** ChatGPT-sourced art (from `book004_approval`)
- **Pages 27–58:** Cursor GenerateImage
- **Pages 1–2 + cover:** ChatGPT / owner-approved (`cover_chatgpt.png` / `APPROVED_COVER_FRONT.png`)
- **Pages 59–63 blanks + 64 colophon:** production assets already at 2550×3300

## Files in this FINAL folder
- `interior/page_001.png` … `interior/page_064.png` — normalized **2550×3300 RGB** (8.5×11 @ 300 DPI)
- `Little_Ones_Little_Builder_INTERIOR_64pp.pdf` — 64 pages, one image per page
- `Little_Ones_Little_Builder_COVER_WRAP.png` — full paperback wrap **5218×3375 px** @ 300 DPI
- `Little_Ones_Little_Builder_COVER_WRAP.pdf` — same wrap as single-page PDF
- `README_FINAL_CHECK.md` — this file

### Cover wrap geometry
- Bleed: 0.125 in each side
- Height: 11.25 in → **3375 px**
- Width: 0.125 + 8.5 + 0.144128 + 8.5 + 0.125 = **17.394128 in** → **5218 px**
- Spine: construction yellow, vertical title + imprint
- Back: construction-themed light panel; **barcode safe zone (~2"×1.2") lower-right of back panel left white**

## Print / DPI notes
- Target interior: 2550×3300 @ 300 DPI
- Source pages 1–26 / cover were ~1102×1427 (~130 DPI native) — **LANCZOS upscaled** to 2550×3300 (near-native aspect → centered cover-crop)
- Source pages 27–58 were 1280×720 landscape — **LANCZOS fit + white letterbox** to 2550×3300 (preserve aspect)
- Upscaled ChatGPT pages will not be true 300 DPI photographic detail; acceptable for B&W line-art coloring at this trim, but owner should soft-proof print quality

## KDP metadata reminders (when owner approves — NOT now)
- AI disclosure tool name: **Cursor** (when KDP field is editable)
- Price: $9.99
- Expanded Distribution: OFF
- **NO publish until owner approves**


## Build notes (package)
- Interior PNGs: **RGB** 2550×3300 as specified
- Interior PDF: JPEG-compressed grayscale embeds @ quality 92 (KDP B&W print intent; keeps file under GitHub 100MB limit). Page count still exactly 64.
- Cover wrap remains full-color RGB

## GitHub review URL
https://github.com/TrippyThrifter/kdp-public-review/tree/main/book_004_Little_Builder_REVIEW

FINAL mirror path in that folder: `FINAL/`

## Update 2026-09-21 evening — pages 27–58 remount
Cursor GenerateImage cannot emit true portrait (always 1280×720). Cover-crop clipped bubble labels.
**Fix applied:** remounted each landscape master into full 8.5×11 with vehicle filling the upper area and the **full noun strip** preserved at the bottom (no letterbox bands, labels intact).
Interior PDF refreshed: `Little_Ones_Little_Builder_INTERIOR_64pp.pdf`
