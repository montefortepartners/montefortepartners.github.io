# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for Monteforte Partners (www.montefortepartners.com), a strategic advisory and financial consulting firm. Hosted via GitHub Pages with a custom domain.

## Architecture

This is a single-page static site with no build system, bundler, or dependencies:

- **`index.html`** — The entire site: HTML structure, embedded CSS (in `<style>`), and inline JavaScript (in `<script>`)
- **`CNAME`** — Custom domain configuration for GitHub Pages (`www.montefortepartners.com`)
- No package.json, no build step, no tests

## Development

Open `index.html` directly in a browser to preview. There is no dev server or build command.

## Deployment

Push to `main` branch — GitHub Pages auto-deploys.

## Design Conventions

- Dark theme using CSS custom properties (`:root` variables: `--bg-dark`, `--bg-section`, `--accent`, etc.)
- Typography: "Playfair Display" for headings, "Inter" for body text (loaded from Google Fonts)
- Gold accent color (`#d4af37`)
- Sections use IntersectionObserver for scroll-triggered fade-in animations
- Mobile-responsive via media query at 768px breakpoint
