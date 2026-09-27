# Prism

One window, every great model. Prism is a chat app for Google's Gemini and Gemma
models, fast open models (like Llama) through Groq, and Mistral's own models.
It's a static site with no build step and no server, so it runs on GitHub Pages.

**Live:** <https://aabs007.github.io/prism/>

## Features

**Chatting**
- Replies stream in as they're written
- Edit a sent message, retry the last reply, copy, or have a reply read aloud
- Voice input: tap the mic and talk
- Attach or paste images and PDFs
- Maths (KaTeX), diagrams (Mermaid), Markdown and code blocks with copy buttons
- Soft send and reply sounds (can be turned off)

**Models and tools**
- The newest Gemini and Gemma models, loaded automatically
- Optional Groq and Mistral keys for more models
- **Search:** Gemini answers from Google Search, with sources
- **Image:** create images with Gemini's image model
- **Compare:** send one message to up to 3 models and see the answers side by side
- **Personas:** Tutor, Code helper, Writer, Translator, Concise, or your own

**Your chats**
- Every conversation is saved in your browser, with search, pin, rename and delete
- Export all chats to a file and import them on another device

**Looks**
- Animated space wallpapers: starfield, black hole, quasar, galaxy, nebula,
  Saturn, supernova, wormhole and aurora (or Auto, which follows light/dark mode)
- Light and dark mode, works on phones
- Installable as an app (home screen or dock), and opens offline

## Use it
1. Get a free API key at <https://aistudio.google.com/apikey>.
2. Open the page, click **⚙ Settings**, and paste your key.
3. Optional: get a free Groq key at <https://console.groq.com/keys>.
4. Optional: get a free Mistral key at <https://console.mistral.ai/api-keys>.

Your keys, settings and chats are saved only in your own browser. Each key is
sent only to its own provider (Google, Groq or Mistral). Keys are **never** put
in this repo, so it's safe for the repo to be public. Each visitor uses their own key.

## Files
- `index.html`: the whole app
- `manifest.webmanifest`, `sw.js`, `icons/`: what lets it install as an app and open offline
- `favicon.svg`: the tab icon

## Put it on GitHub Pages
1. Create a repository on GitHub and upload these files.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*,
   pick `main` and `/ (root)`, then click **Save**.
4. After a minute your site is live at `https://<your-username>.github.io/<repo-name>/`.

## Run locally
Serve the folder (installing and offline mode need a server, not a double-clicked file):

```bash
python3 -m http.server 8000
```
