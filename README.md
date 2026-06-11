# World History — OCS Summer School
### Course Hub · `index.html`

---

## Overview

Student-facing landing page for the OCS Summer School World History course (Standards 10.1–10.11). Opens directly in any browser — no server or build tools required.

---

## Structure

```
/
├── index.html           ← Main course hub (this file)
├── README.md            ← This file
└── images/
    └── header_world.jpg ← Hero banner image (see below)
```

---

## Lesson Files

Naming convention: `SSW_S#L##.html`

### Semester 1 — Ancient Roots Through WWI (Standards 10.1–10.5)

| Day | File             | Title                                      | Standard(s)            |
|-----|------------------|--------------------------------------------|------------------------|
| 1   | SSW_S1L01.html   | Roots of Western Political Thought         | 10.1                   |
| 2   | SSW_S1L02.html   | Democratic Revolutions                     | 10.2                   |
| 3   | SSW_S1L03.html   | The Industrial Revolution                  | 10.3                   |
| 4   | SSW_S1L04.html   | New Imperialism                            | 10.4                   |
| 5   | SSW_S1L05.html   | Causes of World War I                      | 10.5 pt. 1             |
| 6   | SSW_S1L06.html   | Fighting WWI                               | 10.5 pt. 2             |
| 7   | SSW_S1L07.html   | The Human Cost of WWI                      | 10.5 pt. 3             |
| 8   | SSW_S1L08.html   | Nationalism and the Long Road to WWI       | 10.2 pt. 2 / 10.5      |
| 9   | SSW_S1L09.html   | The World WWI Left Behind                  | 10.5 continued         |
| 10  | SSW_S1L10.html   | **Semester 1 Final**                       | 10.1–10.5              |

### Semester 2 — WWI Aftermath Through Globalization (Standards 10.6–10.11)

| Day | File             | Title                                      | Standard(s)            |
|-----|------------------|--------------------------------------------|------------------------|
| 1   | SSW_S2L01.html   | The Failed Peace After WWI                 | 10.6                   |
| 2   | SSW_S2L02.html   | Rise of Totalitarian Governments           | 10.7                   |
| 3   | SSW_S2L03.html   | Causes and Start of World War II           | 10.8 pt. 1             |
| 4   | SSW_S2L04.html   | Fighting WWII and the Holocaust            | 10.8 pt. 2             |
| 5   | SSW_S2L05.html   | Post-War World and Cold War Origins        | 10.9 pt. 1             |
| 6   | SSW_S2L06.html   | Cold War Conflicts Around the World        | 10.9 pt. 2             |
| 7   | SSW_S2L07.html   | Decolonization and Nation-Building         | 10.10                  |
| 8   | SSW_S2L08.html   | Globalization and the Information Revolution | 10.11                |
| 9   | SSW_S2L09.html   | The Cold War Ends                          | 10.9 continued         |
| 10  | SSW_S2L10.html   | **Semester 2 Final**                       | 10.6–10.11             |

---

## Card Display Logic

Cards are ordered by instructional relevance each day:

- **Today's card** (Day 5) leads — terracotta `TODAY` badge, highlighted border, spinning star ornament
- **Upcoming cards** (Days 6–9) follow in sequence
- **Completed cards** (Days 1–4) at the end — muted/faded
- **Day 10 Final** always anchors last with `FINAL` badge

To advance to the next day: move that card to the top, apply `class="day-card today"`, update the badge text, and change the pip JS threshold (`i < 5` → `i < 6` for Day 6, etc.).

---

## Header Image

```
FILENAME:  header_world.jpg
FOLDER:    images/
SOURCE:    Wikimedia Commons
TITLE:     "Theatrum Orbis Terrarum" — Abraham Ortelius, 1570
URL:       https://commons.wikimedia.org/wiki/File:OrteliusWorldMap1570.jpg
ALT:       https://commons.wikimedia.org/wiki/File:Mercator_1569.png
```

Download the full-size image and save as `images/header_world.jpg`. Falls back to a dark ink background if missing.

---

## Design Notes

- **Fonts**: Cormorant Garamond (headings, card titles, italic text) + DM Sans (labels, body, badges)
  — elegant Garamond refinement paired with clean modern humanist sans; no heavy serifs or blocky type
- **Color palette**: Muted globe tones — dusty ocean teal (`#4a7a8a`), worn terracotta (`#8a5a3a`),
  faded atlas sand (`#b89a6a`), forest green (`#4a6a48`), slate blue (`#4a5a6a`). All desaturated
  like aged cartographic ink — not vivid, not gray
- **Background**: Warm mid-tone `#eceae5` with subtle SVG grain texture

## JS/CSS Enhancements

- **Scroll-progress bar** — ocean-to-terra gradient, pinned top of page
- **Session progress pips** — dark strip under hero; 4 teal done, 1 white active, 5 dim upcoming
- **Interactive compass** — needle in hero corner rotates to track your cursor position within the hero;
  snaps back on mouse leave with spring easing (cubic-bezier)
- **Region tooltip** — pure CSS `attr()` trick on `data-region`; geographic context fades in top-right
  of each card on hover (e.g. "Europe · 1914", "Africa · Asia", "Korea · Vietnam")
- **Intersection Observer scroll-reveal** — cards stagger in as they enter viewport; done separately
  per grid so Semester 1 and Semester 2 each stagger independently
- **Today card spinning star** — the `✦` corner ornament rotates continuously on today's card

---

*World History · OCS Summer School · SSW*
