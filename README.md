# conifer_web

GitHub Pages should publish this site from the `docs/` folder on the default branch.

## Structure

- `docs/`: published website

## Preview locally

From this repository root, run:

`python3 -m http.server 8000 --directory docs`

Then open:

`http://localhost:8000/`

If you run the server on a remote machine, open `http://<remote-host>:8000/` or forward the port with SSH:

`ssh -L 8000:127.0.0.1:8000 <user>@<remote-host>`

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

This site is configured for the custom domain `coniferelectronics.com` via `docs/CNAME`.
