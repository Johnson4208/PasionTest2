# PASION — GitHub Pages version

This is the **static GitHub Pages frontend** of PASION. The existing React components, SCSS, typography, images, layout, animations, navigation, charts, and interactions are preserved.

## Deploy

GitHub Pages cannot execute server-side Python, PHP, or Ruby. PASION therefore uses Vite to compile the React/SCSS source into static HTML, CSS, and JavaScript, while `src/staticApi.js` provides browser-local demo behavior for the original `/api` calls. GitHub's documentation recommends a GitHub Actions build for non-Jekyll static site generators. 

1. Push the contents of this folder to the **root of your GitHub repository**.
2. Open **Settings → Pages**.
3. Set **Source = GitHub Actions**.
4. Push to `main`, or run **Deploy PASION to GitHub Pages** manually under the Actions tab.
5. Open the Pages URL shown by GitHub.

**Do not choose “Deploy from a branch” for this source tree.** That would serve the JSX/SCSS source directly instead of running Vite and commonly produces a white page.

## Local frontend preview

```bash
npm install
npm run build:github
npm run preview:github
```

## Static demo account

Email: `demo@solvai.com`  
Password: `SolvAI2024!`

Account registration/session data is stored only in the current browser. Secure authentication, password recovery, SMTP email, document upload/OCR, and server-side administration require a separate backend deployment.
