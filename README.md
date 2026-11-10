# Minjoon Kee — CV

A responsive, two-column CV website for GitHub Pages. Plain HTML, CSS, and a short script for printing; no dependencies or build step. Contact details and education sit in a sidebar, with the profile and research experience in the main column. The layout stacks on small screens and keeps two columns when printed.

## Update the CV

Edit `index.html` to change the biography, research experience, education, publications, or links. Publication citations use ACL Anthology metadata; downloadable BibTeX files are in `publications/`. Change `styles.css` to adjust the appearance. The **Print / PDF** button opens the browser print dialog; choose **Save as PDF** to export the CV.

The favicon is a saved copy of the GitHub avatar for `Ariaspect`, stored at `assets/github-avatar.png`. Replace this file to update the favicon after changing the profile picture.

The sidebar portrait is the supplied photo, stored unchanged at `assets/portrait.jpg`. Its display size is controlled by the `.portrait` rules in `styles.css`.

## Font

The site serves JetBrains Mono Nerd Font Mono in regular and bold weights from `assets/fonts/`, so visitors do not need the font installed. The WOFF2 files retain the font’s Nerd Font glyphs. Source: [Nerd Fonts / JetBrains Mono](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/JetBrainsMono/Ligatures). The SIL Open Font License is included in `assets/fonts/OFL.txt`.

## Publish on GitHub Pages

1. Use a public repository named `ariaspect.github.io` under the `Ariaspect` account.
2. Commit these files to the `main` branch, with `index.html` at the repository root.
3. In **Settings → Pages**, select **Deploy from a branch**, then **main** and **/ (root)**, and save.
4. GitHub publishes the site at https://ariaspect.github.io/. Subsequent commits to `main` update the site automatically.

The `.nojekyll` file makes GitHub serve the static files directly. No GitHub Actions workflow or package installation is required.

## Preview locally

From the repository directory:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 in your browser.
