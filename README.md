# Investor Deck Generator

Static investor presentation deck for **Dugout Howe Complex**, a youth sports facility project in Howe, TX, operated by **Pine Tar Sports**.

This repository contains a browser-based slide deck built with plain HTML and CSS. Each slide is a standalone file, connected through previous/next navigation buttons.

## Project Purpose

The deck is used to present the investment opportunity, including:
- Business overview and market demand
- Facility concept and development phases
- Revenue model and financial projections
- Investment structure and ownership opportunities
- Call to action for prospective investors

## Tech Stack

- Static HTML (one file per slide)
- Shared CSS stylesheet (`manus.css`)
- No JavaScript framework, build step, or backend
- CDN dependencies:
  - Font Awesome 6.0.0-beta3
  - Google Fonts (Montserrat + Open Sans via `@import` in `manus.css`)

## Repository Structure

- `index.html` - Cover / title slide
- `slide-01.html` to `slide-10.html` - Main content slides
- `slide-01a.html`, `slide-09-1.html` - Inserted sub-slides
- `manus.css` - Shared base styling, brand variables, responsive behavior
- `images/` - Slide image assets
- `vercel.json` - Static hosting configuration for Vercel

## Slide Sequence (Current Navigation)

Based on each slide's previous/next links:

1. `index.html`
2. `slide-01.html`
3. `slide-01a.html`
4. `slide-02.html`
5. `slide-07.html`
6. `slide-08.html`
7. `slide-09.html`
8. `slide-09-1.html`
9. `slide-03.html`
10. `slide-04.html`
11. `slide-05.html`
12. `slide-10.html`

> Note: `slide-06.html` currently exists in the repo but is not connected in the live previous/next navigation flow.

## Design and Layout Notes

- Target slide canvas: **1280x720** (16:9)
- Shared brand/color variables are defined in `:root` inside `manus.css`
- Slide-specific styling is typically embedded in a `<style>` block inside each slide file
- Responsive behavior is included for narrower viewports (down to 480px)

## Financial and Compliance Language

When editing financial copy, use compliance-safe phrasing:
- Use **"target"** or **"projected"**
- Avoid language implying guaranteed returns

## Run Locally

You can open `index.html` directly in a browser, or serve the folder locally for consistent relative-asset loading:

```bash
cd /Users/larryontruman/Desktop/Coding/investor-deck-generator
python3 -m http.server 8080
```

Then visit:
- `http://localhost:8080/index.html`

## Deploy

This project is configured as a static site on Vercel (`vercel.json` sets output directory to `.`).

## Editing Guidelines

- Keep one slide per HTML file
- Preserve linear previous/next navigation
- Reuse `manus.css` variables for colors and shadows
- Avoid adding new dependencies unless explicitly approved
- Keep copy and investment figures consistent across slides

## Contact Context in Deck

The presentation identifies:
- **Tim Truman**
- **Pine Tar Sports**
- **491 Morrison Rd, Howe, TX 75459**
