# Gemini Chat

A simple, single-page chat interface for Google's Gemini models. It's a single
`index.html` file with no build step and no server, so it works on GitHub Pages.

## Features
- Streams replies as they're written
- Choose any Gemini model your key can access (the list loads automatically)
- Attach or paste images
- Markdown and code blocks, with copy buttons
- Optional system instructions and temperature setting
- Light and dark mode, and it works on phones

## Use it
1. Get a free API key at <https://aistudio.google.com/apikey>.
2. Open the page, click **⚙ Settings**, and paste your key.

Your key is saved only in your own browser (localStorage) and is sent only to
Google's API. It is **never** put in this repo, so it's safe to make the repo public.
Each visitor enters their own key.

## Put it on GitHub Pages
1. Create a new repository on GitHub and upload `index.html` (and this README).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*,
   pick `main` and `/ (root)`, then click **Save**.
4. After a minute your site is live at `https://<your-username>.github.io/<repo-name>/`.

## Run locally
Just double-click `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
```
