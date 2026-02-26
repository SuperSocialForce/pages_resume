# Resume Page

Simple single-page resume template published with GitHub Pages. Customize the content under `site/` and push to `main`; the included workflow deploys to Pages automatically.

## Getting started

1. **Update the template**
   - Edit `site/index.html` with your actual name, contact links, experience, projects, and education.
   - Adjust colors or layout in `site/styles.css`. Keep the markup semantic for accessibility.
2. **Preview locally**
   - Open `site/index.html` directly in a browser, or run a lightweight server such as `python3 -m http.server --directory site 3000`.
3. **Commit and push**
   - Initialize git (if you haven't) and push to a GitHub repo on the `main` branch.

```bash
git init
git add .
git commit -m "Set up resume page"
git branch -M main
git remote add origin git@github.com:<username>/resume_page.git
git push -u origin main
```

## Deploy to GitHub Pages

Once the repository is on GitHub:

1. Navigate to **Settings → Pages** and ensure the source is set to **GitHub Actions**.
2. The `Deploy to GitHub Pages` workflow (in `.github/workflows/deploy.yml`) builds nothing and uploads the `site/` directory as the artifact.
3. After the workflow completes, the live URL is shown in the workflow summary and under **Settings → Pages**.

## Customization ideas

- Replace the SVG avatar with your own photo or illustration.
- Duplicate the `card` component to list more roles or projects.
- Add JSON data and a small build step if you later want to auto-generate sections.
