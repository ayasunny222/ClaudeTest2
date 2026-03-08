# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of self-contained HTML web pages — no build tools, no dependencies, no server required. Each file runs directly in the browser.

## Files

- `tictactoe.html` — Tic Tac Toe game (two-player and vs minimax AI)
- `horoscope-march.html` — Jingya's Magic Horoscope Newsletter (March 2026, all 12 signs)
- `tarot-newsletter.html` — Celine's Newsletter (weekly tarot reading, March 7–14 2026)

## Development

Open any file directly in a browser:
```
file:///C:/Users/PC/Documents/data%20analytics/ClaudeTest2/<filename>.html
```

Or launch via PowerShell:
```powershell
powershell.exe -Command "Invoke-Item '<absolute-path-to-file>'"
```

## Architecture

Each HTML file is fully self-contained: HTML structure, `<style>` block for CSS, and `<script>` block for JavaScript — all in one file. There are no external JS libraries; Google Fonts is the only external resource (loaded via `@import` in CSS).

## Git & GitHub

Repository: https://github.com/ayasunny222/ClaudeTest2

Workflow for every change:
1. Edit the file
2. `git add <file>` — stage only the changed file (never `git add .`)
3. `git commit -m "..."` — descriptive message, present tense, max ~72 chars
4. `git push` — push to GitHub immediately after committing

Each file gets its own commit. Do not batch unrelated files into one commit.
