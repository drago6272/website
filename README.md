# Teddy's Portfolio Site

This is a very simple static site to show off projects and things you've built in your spare time. It uses just plain HTML, CSS, and a tiny bit of JavaScript.

## Files

- `index.html` – main page with sections for About, Projects, and Contact
- `styles.css` – styling for the layout and cards
- `script.js` – sets the current year in the footer

## Editing the content

Open `index.html` in any text editor and look for:

- The **hero section** for the main intro text
- The **Projects** section for the individual project cards
- The **Contact** section for your email, GitHub, and other links

You can duplicate a `.project-card` block to add more projects.

## Previewing the site locally

### Easiest: open the file directly

From your file manager, double‑click `index.html`. Your browser will open it from your filesystem, and you can refresh after edits. This is good enough for basic layout/content changes.

### Recommended: run a tiny local web server

From the `website` folder:

```bash
cd /home/teddy/Documents/website
python3 -m http.server 8000
```

Then open this URL in your browser:

```text
http://localhost:8000
```

Leave that terminal running while you work. Any time you edit and save the files, just refresh the browser tab.

To stop the server, go back to the terminal and press `Ctrl + C`.

## Publishing with GitHub Pages (optional)

1. Create a new public repo on GitHub, e.g. `teddy-portfolio`.
2. From this folder, initialize git and push:

   ```bash
   cd /home/teddy/Documents/website
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin git@github.com:YOUR_USERNAME/teddy-portfolio.git
   git push -u origin main
   ```

3. In the GitHub repo settings, enable **GitHub Pages** for the `main` branch and root (`/`) folder.
4. GitHub will give you a URL where the site is hosted.

