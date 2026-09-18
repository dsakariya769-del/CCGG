# MindSync — Decision Lab

This is a React + Vite dashboard for exploring a topic/thought dump with two AI models.

## IMPORTANT: GitHub Pages

Do **not** upload this project and select the normal "Deploy from branch / root" option.  
This is a Vite source project, so GitHub must first run `npm install` and `npm run build`.

This ZIP now includes a GitHub Actions workflow that does that automatically.

### Exact steps

1. Create/open a GitHub repository.
2. Upload **all files and folders inside this ZIP** to the repository root.
3. Make sure `.github/workflows/deploy.yml` is also uploaded.
4. Commit/push to the `main` branch.
5. Open **Settings → Pages**.
6. Under **Build and deployment → Source**, select **GitHub Actions**.
7. Go to the repository's **Actions** tab.
8. Wait for **Deploy to GitHub Pages** to finish successfully.
9. Open the Pages URL shown by GitHub.

### Why the old version showed white

The old ZIP was the React source code. GitHub Pages was trying to serve `index.html` directly, but the browser cannot execute the unbuilt JSX/Vite source as a production website. The new workflow builds it first.

## Local development

```bash
npm install
npm run dev
```

## API keys

This V1 uses browser-side BYOK settings and LocalStorage. Do not put a valuable production API key into a public repository or source file.
