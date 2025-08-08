# Personal Portfolio Site

> A space-themed portfolio site with solar system animation and comprehensive documentation

## Quick Start

To run the site locally:
```bash
# Using Python 3
python -m http.server 8000

# Or using Node.js
npx http-server
```

Then visit `http://localhost:8000` in your browser.

## Directory Structure

```
altsite2/
│
├── index.html                  # Main landing page with solar system animation
├── docs.html                   # Docsify documentation viewer
├── _sidebar.md                 # Navigation structure for documentation
├── README.md                   # This file
├── NASALIZA.TTF               # NASA font file for title display
│
├── Asteroid Destroyer/         # Minigame (activated by clicking satellite)
│   └── index.html             # Game entry point
│
└── docs/                      # All documentation content in markdown
    ├── introduction.md        # Welcome/intro page
    │
    ├── academic/              # Academic section
    │   ├── profile.md
    │   ├── institutions/      # Educational institutions
    │   │   ├── mast-academy.md
    │   │   ├── university-of-florida.md
    │   │   ├── thomas-jefferson.md
    │   │   └── ua-medicine.md
    │   ├── experiences/       # Academic experiences
    │   │   ├── hanson-lab.md
    │   │   ├── itolerance.md
    │   │   └── science-advocacy-uci.md
    │   └── projects/          # Academic projects
    │       ├── hemoglobin-pmf.md
    │       ├── human-speciation.md
    │       ├── ehr-space.md
    │       ├── med-sim-engine.md
    │       ├── biostats-education.md
    │       └── wetware-policy.md
    │
    ├── operational/           # Operational section
    │   ├── profile.md
    │   └── skills/           # Technical/field skills
    │       ├── diving.md
    │       ├── radio.md
    │       ├── flying.md
    │       ├── ropework.md
    │       └── search-rescue.md
    │
    ├── professional/          # Professional section
    │   ├── profile.md
    │   ├── experiences.md
    │   └── experiences/      # Work experiences
    │       ├── sanaby-health.md
    │       ├── japour-enterprises.md
    │       ├── rosenbloom-lab.md
    │       └── uphs-ma.md
    │
    └── creative/             # Creative section
        ├── profile.md
        └── projects/         # Creative projects
            ├── p521-story.md
            ├── red-rock-diaries.md
            ├── tangency.md
            ├── curiosity-is.md
            ├── research-radar.md
            ├── swift-safari.md
            └── nuyu-sleep-system.md
```

## Key Files to Edit

### Main Landing Page (`index.html`)
- **Hero Section** (lines 855-858): Name and subtitle text
- **Navigation Button** (line 861): "My Life" button
- **Sun Position** (line 1035): Adjust `initialSunContainerY` value
- **Planet Positions** (lines 523-658): Individual planet styling and positions
- **NASA Font** (lines 9-14): Font face definition
- **Color Scheme** (lines 21-29): CSS variables for theming

### Documentation Site (`docs.html`)
- Docsify configuration
- Theme and plugin settings
- Search functionality

### Navigation (`_sidebar.md`)
- Main navigation structure
- Add/remove sections and pages
- Organize content hierarchy

## Adding New Content

### To add a new documentation page:
1. Create markdown file in appropriate `docs/` subdirectory
2. Add link to `_sidebar.md`
3. Follow existing markdown format

### To modify the solar system animation:
- Planet data and info cards: lines 1041-1114 in `index.html`
- Orbital animations: CSS keyframes starting at line 368
- Sun effects: lines 328-396

## Interactive Elements

- **Satellite**: Click to launch Asteroid Destroyer game
- **Sun**: Click to create solar flares
- **Planets**: Hover for information cards
- **Scroll**: Parallax effect moves through solar system

## Technologies Used

- **Docsify**: Markdown-based documentation generator
- **Vanilla JavaScript**: All animations and interactions
- **CSS3**: Complex animations and parallax effects
- **HTML5**: Semantic structure

## Customization Tips

- Adjust planet sizes by modifying width/height in their individual CSS (lines 523-658)
- Change animation speeds by adjusting `animation-duration` values
- Modify color scheme using CSS variables at the top of the file
- Add new planets by following the existing pattern and adding to `planetData` object

## Notes

- The site is designed for GitHub Pages deployment
- All paths are relative for easy hosting
- Mobile responsive with appropriate viewport settings
- Uses CDN for Docsify dependencies