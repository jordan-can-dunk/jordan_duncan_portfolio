# Jordan Duncan — Retro Desktop Portfolio

**Live site:** https://jordan-duncan-portfolio.vercel.app/

A personal portfolio built as a pink, retro Windows-style desktop. Visitors double-click icons to open draggable windows for my resume, projects, and a few things about me.

## How I built this

I created my portfolio to feel like a pink, retro Windows desktop with windows, folders, a media player, and stickers because I wanted a more interactive, personal resume. I built it with AI tools:

1. **Designed and coded with [Claude Design](https://claude.ai).** I described each screen, window, and interaction I had in mind to Claude Design. I used prompt engineering and pintrest reference pictures to describe what I wanted and I iterated with Claude Design until it matched what I'd pictured. 
2. **Reviewed and cleaned up with [Claude Code](https://claude.com/claude-code).** I used Claude Code to check the exported app, remove unused files and drafts left behind by the export, organize the assets into a clear folder structure, and set up deployment on Vercel.


## What's on the desktop

- **About Me**: who I am, plus my inspirations, favorite movies, and trips - this is a fun myspace inspired page I used to describe my personality and interests 
- **Music**: a retro songs player listing my top 10 favorite songs - music is a big part of my life!
- **Movies**: a retro media player listing my top 10 favorite watches - movies are an even bigger part of my life!!
- **Resume**: work experience, academic experience, and skills as retro windows docx. You can download the resume as a `.docx`
- **Projects**: one window per project, with screenshots, write-ups, and links. designed to look like application/cd players and wikipedia about pages

## Project structure

```
.
├── index.html                  # The entire desktop app (markup, styles, and logic)
└── assets/
    ├── vendor/
    │   ├── support.js          # Component runtime (generated; do not edit)
    │   └── image-slot.js       # <image-slot> web component
    ├── documents/
    │   └── Jordan_Duncan_Resume.docx
    └── images/
        ├── wallpaper.png
        ├── icons/              # Favicon and home-screen icon
        ├── about/              # Headshot, avatar, stars, stickers, inspirations, trips
        ├── movies/             # Movie posters
        └── projects/           # Screenshots, one folder per project
```

## Running locally

This is a static site with no build step. Serve the repo root with any static file server:

```bash
git clone https://github.com/jordan-can-dunk/jordan_duncan_portfolio.git
cd jordan_duncan_portfolio
python -m http.server 8000
```

Then open http://localhost:8000.

> Use a local server instead of opening `index.html` straight from disk, since the runtime and YouTube players expect to be served over HTTP.

## Deployment

The site is hosted on Vercel and deploys automatically on every push to `main`. The project uses the **Other** framework preset, no build command, and the repo root as the root directory.

## Built with

- [Claude Design](https://claude.ai) for design and code generation
- [Claude Code](https://claude.com/claude-code) for code review, cleanup, and deployment setup
- HTML, CSS, and JavaScript, rendered by a small React-based component runtime (`assets/vendor/support.js`)
- Google Fonts: Comic Neue, Silkscreen, and Pixelify Sans
- YouTube IFrame API for the music and movie players

## Contact

Jordan Duncan · [GitHub @jordan-can-dunk](https://github.com/jordan-can-dunk)
