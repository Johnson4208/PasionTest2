# PASION on GitHub Pages

This package is the static-hosting version of PASION. The UI source and styles are preserved; the Python backend is not executed by GitHub Pages.

## Publish
1. Put the contents of this ZIP at the root of the GitHub repository.
2. Push to `main`.
3. In **Settings → Pages**, choose **GitHub Actions**.
4. The workflow in `.github/workflows/deploy.yml` installs dependencies, runs `vite build`, and publishes `dist/`.

## Demo credentials
- Email: `demo@solvai.com`
- Password: `SolvAI2024!`

The static compatibility layer uses localStorage for the demo session and account creation. Real authentication, email, password recovery, secure document processing, and other server-side operations still require the original Python backend or a separate hosted API.
