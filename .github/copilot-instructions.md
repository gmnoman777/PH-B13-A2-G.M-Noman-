# TechWave Podcast Website - AI Agent Instructions

## Project Overview
This is a static HTML/CSS website for the TechWave podcast, featuring a single-page landing page with hero, about, features, and featured episodes sections. No JavaScript or build tools required - edit files directly and open `index.html` in a browser to preview.

## Architecture
- **Single Page Structure**: All content in `index.html` with `<header>`, `<main>` containing `<section>` elements
- **Styling**: Centralized in `styles.css` using CSS Grid and Flexbox
- **Assets**: Images stored in `images/` folder, referenced with relative paths
- **External Dependencies**: Google Fonts (Inter), Font Awesome icons, YouTube iframes for episodes

## Key Patterns & Conventions

### HTML Structure
- Use semantic elements: `<header>`, `<main>`, `<section>`, `<nav>`
- Navigation: `<nav>` with `.logo`, `.menu` (flex list), `.btn` subscribe button
- Sections: Class `.section-div` for dark background sections, `.hero` for full-width hero
- Content containers: `.about-container` (flex), `.Choose-container` (CSS Grid 3x3), `.episode-container` (CSS Grid 3 columns)

### Styling Patterns
- **Typography**: Inter font family, weights 400-900, line-heights for readability
- **Color Scheme**: 
  - Background: `#1A0B2E` (dark purple)
  - Text: `#FFFFFF` (white), `rgba(255,255,255,0.788)` (muted white)
  - Accent: `#00FF88` (green) for highlights and secondary buttons
  - Branding gradient: `linear-gradient(45deg, #F7E93F,#FB09B4,#9100F8)` for logo and primary buttons
- **Buttons**: `.btn` class for primary (gradient bg), `.subs` for secondary (green border)
- **Layout**: Flexbox for horizontal alignment, CSS Grid for complex layouts (e.g., `.Choose-container` with `grid-template-columns: repeat(3,1fr)`)
- **Spacing**: Consistent padding (e.g., 120px vertical for sections), gaps (30px for grids)

### Adding Content
- **New Episodes**: Add `<div class="episode-card">` inside `.episode-container` with `<iframe>` (YouTube embed), `.card-content` div containing `<h6>`, `<p class="paragraph">`, `<span>` with duration
- **New Features**: Add `<div class="Choose-content">` in `.Choose-container` grid, include `<img>`, `<h6>`, `<p class="paragraph">`
- **Images**: Place in `images/` folder, use relative paths like `images/filename.png`

### Development Workflow
- Edit `index.html` for content, `styles.css` for styling
- Preview: Open `index.html` in browser (no server needed)
- No build process or dependencies to install
- Maintain responsive design principles (though currently desktop-focused with fixed widths)

## Examples
- Hero button: `<button class="btn"><i class="fa-brands fa-spotify"></i> Listen on Spotify</button>`
- Episode card title: `<h6>The Future of AI in Everyday <br> Life</h6>`
- Grid item sizing: `.small-medium { grid-row: span 2; }` for taller feature cards</content>
<parameter name="filePath">c:\projects\PH-B13-A2-G.M-Noman\.github\copilot-instructions.md