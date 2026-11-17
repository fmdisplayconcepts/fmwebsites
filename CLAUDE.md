# fmwebsites

- Each folder in `sites/` is a separate, self-contained static website (plain HTML/CSS/JS, no build step, no Node.js). Never reference files across site folders.
- New sites start as a copy of `sites/_template/`.
- Every page repeats the same header/nav/footer; when adding or renaming a page, update the nav in every page of that site and set `aria-current="page"` on the current one.
- Rebrand via the `:root` variables in each site's `css/style.css`.
- Preview: `python3 -m http.server 8000 --directory sites`, then open `/<site-folder>/`.
- Work on a branch and open a pull request; don't commit to `main`.
