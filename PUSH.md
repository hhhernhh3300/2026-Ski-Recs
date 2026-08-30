# Two commands to go live

## 1. Create the repo on GitHub
https://github.com/new  →  name it `ski-cards-dec-2026`  →  **do not** tick
"Add a README" (this folder already has one)  →  Create.

## 2. Push (run these in this folder)
Replace YOURNAME with your GitHub username.

```bash
git remote add origin https://github.com/YOURNAME/ski-cards-dec-2026.git
git push -u origin main
```

The commit is already made. Nothing else to stage.

## 3. Connect Cloudflare Pages
Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git → pick the repo.
Framework preset **None**, build command **blank**, output directory **`/`** → Save and Deploy.

Live at `https://ski-cards-dec-2026.pages.dev` in about a minute, and every
`git push` after that redeploys on its own.
