# fmwebsites

Websites built and maintained by FM Display Concepts. Each site is plain HTML, CSS and JavaScript: no build step, no Node.js, nothing to install beyond git.

## Layout

```
sites/
  _template/           starter files: copy this to begin a new site
  fmdisplayconcepts/   FM Display Concepts company site
    index.html         one .html file per page
    css/style.css      styles; rebrand by editing the colors/fonts in :root
    js/main.js         mobile menu + footer year
    images/            photos, logos, icons
```

Each folder in `sites/` is a complete, self-contained website that can be hosted on its own.

## Preview a site on your Mac

From the repo folder:

```bash
python3 -m http.server 8000 --directory sites
```

Then open http://localhost:8000/fmdisplayconcepts/ in your browser. Press Ctrl+C in the terminal to stop.

## Start a new site

```bash
cp -R sites/_template sites/new-site-name
```

Then edit `sites/new-site-name/index.html` (title, logo text, content) and the `:root` colors in `css/style.css`. Use lowercase folder names with dashes.

## Working as a team

1. Get the latest: `git pull` on `main`.
2. Make a branch for your change: `git switch -c your-name/what-you-are-changing`.
3. Commit and push your branch, then open a pull request on GitHub.
4. Someone else reviews it, then it gets merged into `main`.

Don't commit straight to `main`.
