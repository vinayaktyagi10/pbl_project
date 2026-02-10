# SDC Infrastructure Automation - PBL Presentation

This is a web-based presentation built with [Reveal.js](https://revealjs.com/). It functions like a PowerPoint but runs in a web browser using HTML, CSS, and JavaScript.

## Features
- **Auto-Timer:** A countdown timer (top-right) starts automatically when you change the first slide. It turns orange at 2 mins left and red at 30 seconds left.
- **Code Highlighting:** Optimized for showing Bash and JavaScript snippets.
- **Mobile Responsive:** Works on phones and tablets.

## How to View Locally
1. Simply double-click `index.html` to open it in your browser.
2. Press `F11` for Full Screen mode.
3. Use Arrow Keys or Spacebar to navigate.

## How to Deploy to GitHub Pages
1. Push this folder to a GitHub repository.
2. Go to **Settings** > **Pages**.
3. Under **Branch**, select `main` (or `master`) and keep the folder as `/ (root)`.
4. Click **Save**.
5. Wait ~1 minute, and your presentation will be live at `https://your-username.github.io/repo-name/`.

## Customization
- **Edit Content:** Open `index.html` in a text editor (VS Code, Notepad, etc.).
- **Change Timer:** Search for `let totalTime = 10 * 60;` in `index.html` and change `10` to your desired minutes.
