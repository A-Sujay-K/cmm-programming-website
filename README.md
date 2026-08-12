# CMM Programming Services — Website

A bespoke, editorial-style landing page designed for a high-end precision metrology and CMM programming service provider operating in the UK and Ireland.

## Architecture & Tech Stack

This project deliberately avoids heavy frameworks and "cookie-cutter" templates to maintain a premium, custom-engineered feel.

*   **HTML5 & CSS3:** Pure, semantic markup with native CSS variable tokenization for colors and typography.
*   **Typography:** [Instrument Serif](https://fonts.google.com/specimen/Instrument+Serif) (for precision/editorial headings) and [Geist / Geist Mono](https://vercel.com/font) (for technical data and labels).
*   **Animation:** [GSAP (GreenSock)](https://gsap.com/) and ScrollTrigger for buttery smooth, physics-based scroll reveals that outperform standard CSS transitions.
*   **Assets:** Custom generated, monochromatic precision engineering photography.

## Local Development

To run the site locally, simply serve the directory using any local web server. For example, with Python 3:

```bash
python -m http.server 8080
```
Then navigate to `http://localhost:8080`.

## Customization Guide

All company-specific data has been parameterized using bracket notation in the `index.html` file. Search for the following strings to replace them with live data:

*   `[Company Name]` — e.g. ARC Metrology
*   `[Phone Number]` — e.g. 0330 043 7703
*   `[Contact Email]` — e.g. info@arcmetrology.co.uk
*   `[Company Address]`
*   `[City, Region, Postcode]`
*   `[Year]` — Year established, e.g. 2004

### Design Tokens
Colors and fonts are managed via CSS variables in the `:root` pseudo-class at the top of the `<style>` block:

```css
:root {
  --paper:   #F7F4EF;
  --ink:     #141210;
  --mid:     #5C5751;
  --faint:   #C8C3BC;
  --rule:    #D6D0C8;
  --red:     #C0392A; /* Primary accent color */
}
```

## Structure
- `index.html` — The single-page application and all styles/scripts.
- `assets/` — Contains all optimized imagery used on the site.
