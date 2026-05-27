<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/8aa7cdfc-b8c5-4c40-90be-5fef483f1d4a

## Run Locally

**Prerequisites:**  Node.js

1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Deploy to a website

1. Build the production site:
   `npm run build`
2. Deploy the generated `dist/` folder to any static host.

### Deploy with GitHub Pages

- Install dependencies if needed:
  `npm install`
- Run:
  `npm run deploy`

### GitHub Actions auto deploy

- Push to `main` and GitHub Actions will build and deploy to the `gh-pages` branch automatically.
- The workflow file is located at `.github/workflows/deploy.yml`.

### Live GitHub Pages URL

- After deployment, your site will be available at:
  `https://<github-username>.github.io/<repo-name>/`
- Replace `<github-username>` and `<repo-name>` with your account and repository names.

### Deploy to Netlify

- Connect the repo in Netlify.
- Set build command to `npm run build`.
- Set publish directory to `dist`.

### Deploy to Vercel

- Connect the repo in Vercel.
- Use build command `npm run build`.
- Use output directory `dist`.
