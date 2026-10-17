# Jordan Duncan — Retro Desktop Portfolio

A personal portfolio built as a pink, retro Windows-style desktop. Visitors double-click icons to open draggable windows for my resume, projects, and a few things about me.

## What's on the desktop

- **About Me / My World**: who I am, plus my movies, music, inspirations, and trips
- **Resume**: work experience, academic experience, and skills. The resume can be printed or downloaded as a `.docx`
- **Projects**: one folder per project, with screenshots and links
- **My Computer** and **Trash**, for the full desktop feel

## Featured projects

| # | Project | Link |
|---|---------|------|
| 1 | KC Intern Map | [kc-intern-map.dimin.io](https://kc-intern-map.dimin.io/) |
| 2 | Agent Fluffy Bunny | [agent-fluffy-bunny.vercel.app](https://agent-fluffy-bunny.vercel.app/) |
| 3 | Bank Appointment Booking System | [GitHub repo](https://github.com/jordan-can-dunk/commerce-bank-appointment-creator) |
| 4 | Barbie Hangman: Dress Up & Guess | [barbie-hangman.vercel.app](https://barbie-hangman.vercel.app/) |
| 5 | Valentine Candy Battle | [valentine-candy-battle.vercel.app](https://valentine-candy-battle.vercel.app/) |

## Project structure

```
desktop/                      # Deployable site
  index.html                  # Main portfolio desktop
  support.js, image-slot.js   # Runtime scripts the page needs
  *.png, *.docx               # Screenshots, wallpaper, resume
pink-desktop-portfolio.html   # Single-file bundled version (all assets inlined)
Desktop.dc.html               # Source design file
Resume style *.dc.html        # Resume design variations
insp/ stars/ stickers/ trips/ # Images used on the "About Me" pages
```

## Running locally

Clone the repo and serve the `desktop/` folder with any static file server:

```bash
git clone https://github.com/jordan-can-dunk/jordan_duncan_portfolio.git
cd jordan_duncan_portfolio/desktop
python -m http.server 8000
```

Then open http://localhost:8000.

You can also just open `pink-desktop-portfolio.html` in a browser. It's fully self-contained.

## Built with

Plain HTML, CSS, and JavaScript. No build step is needed. Fonts are Comic Neue, Silkscreen, and Pixelify Sans from Google Fonts.

## Contact

Jordan Duncan · [GitHub @jordan-can-dunk](https://github.com/jordan-can-dunk)
