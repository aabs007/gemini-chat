# Prism

One window, every great model. A simple, single-page chat interface for Google's Gemini and Gemma models, plus
fast open models (like Llama) through Groq and Mistral's own models. It's a single
`index.html` file with no build step and no server, so it works on GitHub Pages.

## Features
- Streams replies as they're written
- Choose the newest Gemini and Gemma models (the list loads automatically)
- Optional: add a free Groq key for fast open models like Llama
- Optional: add a free Mistral key for Mistral's models
- Attach or paste images and PDFs
- Animated background: a starfield in dark mode, drifting light in light mode
- Markdown and code blocks, with copy buttons
- Optional system instructions and temperature setting
- Light and dark mode, and it works on phones

## Use it
1. Get a free API key at <https://aistudio.google.com/apikey>.
2. Open the page, click **⚙ Settings**, and paste your key.
3. Optional: get a free Groq key at <https://console.groq.com/keys> and paste it too.
4. Optional: get a free Mistral key at <https://console.mistral.ai/api-keys> and paste it too.

Your keys are saved only in your own browser (localStorage). Each key is sent
only to its own provider (Google, Groq or Mistral). Keys are **never** put in
this repo, so it's safe to make the repo public.
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
