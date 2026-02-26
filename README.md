# Resume Page

Simple single-page resume published with GitHub Pages, with content authored in Markdown.

You only edit `site/resume.md`; the page loads and renders it automatically.

## Getting started

1. **Update the template**
   - Edit `site/resume.md` with your actual name, contact links, experience, projects, and education.
   - Optional: adjust presentation in `site/styles.css`.
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

## Markdown structure tips

- Use `#` for your name, then a short summary paragraph.
- Use `##` for sections like Experience, Projects, Skills, Education.
- Use `###` for each role/project entry.
- Use bullet lists for impact statements.
