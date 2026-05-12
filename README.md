# djlinker-callback (GitHub Pages)

This folder is meant to become its **own** public GitHub repo **`Jboltle/djlinker-callback`**, so Pages serves:

**https://Jboltle.github.io/djlinker-callback/**

`index.html` is a copy of `public/oauth-callback.html` from this project (re-copy after edits to that file).

## One-time: create the GitHub repo and push

```bash
cd deploy/djlinker-callback
git init -b main
git add index.html .nojekyll README.md
git commit -m "Add SoundCloud OAuth callback for djLinker"
```

Create an **empty** public repository on GitHub named **`djlinker-callback`** under **`Jboltle`**, then:

```bash
git remote add origin https://github.com/Jboltle/djlinker-callback.git
git push -u origin main
```

## Enable Pages

On GitHub: **Settings → Pages → Source**: branch **`main`**, folder **`/ (root)`**.

## SoundCloud + `.env`

Use this exact redirect URI in the SoundCloud app and in `SOUNDCLOUD_REDIRECT_URI`:

`https://Jboltle.github.io/djlinker-callback/`
