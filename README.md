# Aman Vishwakarma: Portfolio

A single-file site (`index.html`) with HTML, CSS and JavaScript. No build step and no dependencies apart from Google Fonts, which fall back to system fonts if they fail to load.

## Run locally

- Double-click `index.html`, or
- Run `python3 -m http.server 8000` in this folder and open http://localhost:8000

## Deploy free on GitHub Pages

1. On GitHub, create a public repository. Name it `aman-452001.github.io` to get the root address, or any name (for example `portfolio`) to get `aman-452001.github.io/portfolio`.
2. Upload `index.html` and `README.md` (Add file, then Upload files), or push from the terminal:
   ```
   git init
   git add .
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/aman-452001/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, open Settings, then Pages. Under Source choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. Wait about a minute. The live address appears at the top of the Pages screen.

Netlify Drop (drag the folder onto app.netlify.com/drop) and Cloudflare Pages also work with no changes.

## Update content

All editable content sits at the top of the `<script>` block in `index.html`, between the "EDIT YOUR CONTENT HERE" markers.

- **Project links:** set `repo` to the project's GitHub URL. Change `status` to `"Completed"` when it is finished. Empty `repo` links to your GitHub profile.
- **Real YouTube videos:** in `VIDEOS`, set `id` to the 11 characters after `v=` in the video URL, `url` to the full video link, and replace `t` (title) and `d` (description). Thumbnails load from YouTube once the site is hosted.
- **Skills:** move items between the two groups in `SKILLS` as your confidence grows.
- **Social links:** edit `SITE` once and every button and card updates.
- **Contact:** the contact section is plain HTML near the bottom of the page. Add an email or other details there only if you want to share them.
- **Link previews:** after hosting, add `<meta property="og:image" content="https://your-site/preview.png">` and a `og:url` tag inside `<head>`.

Commit and push after each change and Pages redeploys automatically.
