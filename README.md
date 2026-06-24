# conifer_web

GitHub Pages should publish this site from the `docs/` folder on the default branch.

## Structure

- `docs/`: published website

## Publish on GitHub Pages

1. Create a GitHub repository.
2. Add the remote:
   `git remote add origin <your-repo-url>`
3. Commit and push:
   `git add .`
   `git commit -m "Prepare site for GitHub Pages"`
   `git branch -M main`
   `git push -u origin main`
4. In GitHub, open `Settings` -> `Pages`.
5. Under `Build and deployment`, choose:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/docs`

Do not add a custom domain while testing. GitHub Pages will publish the site at the default `github.io` URL.
