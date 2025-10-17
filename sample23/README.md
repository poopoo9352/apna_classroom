Apna Classroom — Local site README

Quick start

1. Open the site in your browser:
   - Double-click `index.html` in the `sample23` folder.
   - Or run this from PowerShell:
     Start-Process 'c:\Users\mahim\OneDrive\Desktop\updated\sample23\index.html'

What changed

- All site pages have been moved into the project root (flat structure). You can now open `index.html` from the `sample23` folder and navigate to the other pages directly.
- `style.css` and the `images/` directory are in the project root.

Folder layout (important files)

sample23/
- index.html        # Root entry page (open this)
- Box.html          # Educator tools page
- box2.html         # Student tools page
- Signin.html       # Sign-in page
- student.html      # Student dashboard/demo
- options.html      # Options / settings page
- style.css         # Site stylesheet
- images/           # All images used by the site
- package.json      # Dev script to run a local static server via npx live-server
- .vscode/tasks.json# VS Code task to run the dev server

Dev server

1) Run with npm (no global install required):

  npm start

  This uses `npx live-server` to serve the folder on port 5500 and opens the site in your browser.

2) Run from VS Code: open the Command Palette (Ctrl+Shift+P) -> "Tasks: Run Task" -> "Start live server". This runs `npm start` in a terminal.

Notes

- All pages and assets use root-relative links (e.g., `style.css`, `images/...`). If you move files again, update links accordingly.
- If you'd prefer the site served on a different port, edit `package.json`'s `start` script.

Backup suggestion

- If you want a backup of the previous `sih hackathon` folder, I can create a `backup/` folder and move it there before making further changes.

Next steps I can take

- Add a small QA index page that lists all pages and highlights missing assets.
- Add a simple GitHub Pages-friendly deploy instruction or a GitHub Action to preview the site.
- Configure a different static server (http-server, lite-server) if you prefer.
