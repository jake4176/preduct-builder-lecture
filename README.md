# preduct-builder-lecture

**Live site:** https://jake4176.github.io/preduct-builder-lecture/

## Lotto 6/45 Number Generator (행운의 로또 번호 추첨)

A browser-based simulator that draws Korean Lotto 6/45 numbers with an animated reveal. The interface is in Korean.

### Features

- **1 to 5 sets per draw** (sets A–E; 5 sets = one full ticket)
- **Optional bonus number**: draw 6 numbers, or 6 + 1 bonus
- **Custom filters**
  - Pin up to 5 numbers that must appear in every set
  - Exclude numbers you never want drawn
- **Color-coded balls** by range: 1–10 yellow, 11–20 blue, 21–30 red, 31–40 gray, 41–45 green
- **Sound effects** during the draw (can be turned off)
- **Copy results** to the clipboard in one click
- **Recent draw history**: the last 25 sets, saved in your browser (`localStorage`)

### How it works

Everything is in a single `index.html` file: no build step, no framework, no server. Each set is drawn by shuffling the remaining numbers (Fisher–Yates) after applying your include/exclude filters.

To run it locally, just open `index.html` in a browser.

> This is for fun only. Every draw is random, and no method can predict winning numbers.
