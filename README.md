# Jeascelle Papa Portfolio

A responsive, single-page portfolio for Jeascelle Papa, a video editor and
graphic designer. The site is plain HTML, CSS, and JavaScript and requires no
build step.

## Project files

- `jeascelle.html` — the portfolio website
- `aa00b326-f06c-4d86-a497-f5abe7efb8ef.jpg` — profile portrait
- `Ryza mae.pdf` — downloadable résumé
- `vercel.json` — serves `jeascelle.html` at the root URL

## Preview locally

Open `jeascelle.html` directly in a browser, use VS Code Live Server, or run:

```powershell
py -m http.server 8000
```

Then visit `http://localhost:8000/jeascelle.html`.

## Publish to GitHub

Authenticate GitHub CLI and create the remote repository:

```powershell
gh auth login
gh repo create jeascelle-portfolio --public --source=. --remote=origin --push
```

Use `--private` instead of `--public` if the source should not be public.

## Deploy with Vercel

1. Sign in to Vercel and choose **Add New → Project**.
2. Import the `jeascelle-portfolio` GitHub repository.
3. Select **Other** as the Framework Preset.
4. Leave the Build Command blank and keep the Root Directory as `.`.
5. Deploy. Vercel will serve the site directly with no build step.

Every later push to the repository's `main` branch will trigger a production
deployment. Pull requests and other branches receive preview deployments.

