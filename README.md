# Minjoon Kee — CV

A small, responsive CV website for GitHub Pages. Plain HTML, CSS, and a short script for printing; no dependencies or build step.

## Update the CV

Edit `index.html` to change the biography, research experience, education, links, or last-updated date. Change `styles.css` to adjust the appearance. The **Print / PDF** button opens the browser print dialog; choose **Save as PDF** to export the CV.

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
