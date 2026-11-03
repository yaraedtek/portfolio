# Yared Teklegiorgis Birhane — Portfolio

A fast, static portfolio site: plain HTML and CSS, no build step, no dependencies.
It supports light and dark mode and works on phones.

## Structure

```
.
├── index.html              # page content
├── assets/css/style.css    # all styles and theme colors
├── .github/workflows/      # auto-deploy to GitHub Pages
├── .nojekyll
├── LICENSE
└── README.md
```

## Publish on GitHub Pages

1. Create a new repository on GitHub. For a site at `https://<username>.github.io`, name it `<username>.github.io`.
2. Push this folder:
   ```bash
   git init -b main
   git add .
   git commit -m "Add portfolio"
   git remote add origin https://github.com/<username>/<repo>.git
   git push -u origin main
   ```
3. In the repository, open **Settings → Pages** and set **Source** to **GitHub Actions**.
4. Wait for the "Deploy to GitHub Pages" run in the **Actions** tab. Your site is then live.

## Preview locally

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.

## Customize

- Text: edit `index.html`.
- Colors: change the variables at the top of `assets/css/style.css`.
- Add contact links (email, GitHub, LinkedIn) in the `<footer>` of `index.html`.

## License

MIT, see `LICENSE`.
